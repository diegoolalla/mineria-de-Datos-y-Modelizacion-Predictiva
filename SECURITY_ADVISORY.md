# Security Advisory: nbconvert Vulnerability

## ⚠️ Security Warning

**Date**: January 19, 2026  
**Severity**: High  
**Platform**: Windows

## Vulnerability Details

The nbconvert package (version <= 7.16.6) has an **uncontrolled search path vulnerability** that can lead to unauthorized code execution on Windows systems.

- **Affected versions**: <= 7.16.6 (all current versions)
- **Patched version**: Not yet available
- **CVE**: Pending
- **Impact**: Potential unauthorized code execution on Windows

## Recommended Actions

### For Windows Users (High Priority)

**Option 1: Use Jupyter's Built-in Export (RECOMMENDED)**
```python
# From within the Jupyter notebook interface:
# File → Download as → HTML (.html)
```
This method uses the Jupyter web interface and doesn't invoke nbconvert from the command line, reducing the attack surface.

**Option 2: Use nbconvert with Caution**
If you must use nbconvert from command line:
1. Only run it in a trusted directory
2. Ensure no suspicious files are in your PATH
3. Consider running in a sandboxed environment

**Option 3: Use Alternative Export Methods**
```python
# Export using Jupyter's API
jupyter notebook --execute --to html Codigos_Test_Minería_NombreApellido.ipynb --no-input
```

### For Linux/macOS Users

The vulnerability specifically affects Windows. Linux and macOS users can continue using nbconvert normally, but should stay alert for updates.

### For All Users

1. **Monitor for updates**: Check for nbconvert updates regularly
   ```bash
   pip list --outdated | grep nbconvert
   ```

2. **Subscribe to security advisories**:
   - [PyPI Advisory Database](https://github.com/pypa/advisory-database)
   - [Jupyter Security Announcements](https://jupyter.org/security)

3. **Use virtual environments**: Always work in isolated Python environments
   ```bash
   python -m venv myenv
   source myenv/bin/activate  # On Windows: myenv\Scripts\activate
   pip install -r requirements.txt
   ```

## Mitigation Strategies

### Temporary Workaround for Windows Users

1. **Use Jupyter's Web Interface for Export**
   - Open notebook in Jupyter
   - File → Download as → HTML
   - No command-line tools needed

2. **Manual HTML Generation**
   ```python
   # Alternative: Use nbformat and custom HTML generation
   import nbformat
   from nbconvert import HTMLExporter
   
   # Load notebook
   with open('Codigos_Test_Minería_NombreApellido.ipynb') as f:
       notebook = nbformat.read(f, as_version=4)
   
   # Export to HTML
   html_exporter = HTMLExporter()
   html_exporter.template_name = 'classic'
   (body, resources) = html_exporter.from_notebook_node(notebook)
   
   # Save to file
   with open('Codigos_Test_Minería_NombreApellido.html', 'w', encoding='utf-8') as f:
       f.write(body)
   ```

3. **Docker Container** (Advanced)
   ```bash
   # Run in isolated container
   docker run -it --rm -v $(pwd):/work jupyter/minimal-notebook \
       jupyter nbconvert --to html /work/Codigos_Test_Minería_NombreApellido.ipynb
   ```

## Updated Instructions

### Windows Users
**DO NOT USE**: 
```bash
jupyter nbconvert --to html notebook.ipynb  # ❌ Vulnerable on Windows
```

**USE INSTEAD**:
```
1. Open Jupyter Notebook interface
2. Navigate to your notebook
3. File → Download as → HTML (.html)
4. Save the downloaded file
```

### Linux/macOS Users
You can continue using the standard method:
```bash
jupyter nbconvert --to html Codigos_Test_Minería_NombreApellido.ipynb  # ✅ Safe on Linux/macOS
```

## Timeline

- **2026-01-19**: Vulnerability disclosed
- **TBD**: Patch expected (monitor nbconvert releases)

## References

- [nbconvert GitHub Repository](https://github.com/jupyter/nbconvert)
- [Jupyter Security](https://jupyter.org/security)
- [Python Security Advisories](https://github.com/pypa/advisory-database)

## Contact

For questions about this security advisory, refer to:
- Jupyter Security Team: security@jupyter.org
- nbconvert Issue Tracker: https://github.com/jupyter/nbconvert/issues

---

**Last Updated**: January 19, 2026  
**Status**: Active - No patch available yet

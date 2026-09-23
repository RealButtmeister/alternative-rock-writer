# Source setup and checks

This is an interpreted Python/Tk application; there is no compilation step for normal use. No executable, runtime, user settings, or generated lyrics are included.

```powershell
py -3 -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python alt_rock_writer.py
```

On another platform, activate the virtual environment with its platform-specific command and install Tcl/Tk if Python does not include it. The `.vbs` launcher is Windows-only.

Check syntax without contacting the API:

```powershell
python -m compileall -q alt_rock_writer.py lyric_engine.py song_structure.py
```

Use the source launcher as the supported build workflow. If you package an executable separately, preserve resource paths and use a persistent writable settings directory; frozen one-file extraction directories are not suitable for persistent settings. Packaged executables are not included or validated by this repository's staging checks.

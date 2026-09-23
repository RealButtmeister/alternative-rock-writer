# Alternative Rock Writer

A desktop lyric notebook for alternative rock and grunge. It drafts and revises lyrics, checks blocked and required words, and supports custom arrangements and imported Song Structure JSON.

## Run from source

1. Install Python 3.11 or newer with Tcl/Tk support. On Windows, enable the Python launcher during installation.
2. Open a terminal in this repository.

```powershell
python alt_rock_writer.py
```

On Windows, you can also double-click **Launch Alternative Rock Writer.vbs** after setup. The launcher discovers an installed Python; it contains no machine-specific path.

The Python code uses the standard library. Tkinter is supplied by your Python installation, not by pip. See [BUILD.md](BUILD.md) for environment and validation steps.

## Using the writer

Enter a brief, choose the writing controls and length, then add blocked or wanted words. Use Connection to select a model and enter an API key for the current session, or set `OPENAI_API_KEY` locally. Writing requires network access and API usage; the app sends the brief, word lists, and any draft submitted for rewriting to the provider. It produces text, not audio.

Settings can contain your brief and word lists. They are local and ignored by Git. API keys are not written into settings. Save lyrics only to files you choose, and keep personal drafts and keys out of commits.

The detailed original usage notes are in [README.txt](README.txt).

## License

No project license was included in the source snapshot. This repository does not assign a new license. Any third-party components retain their own terms.

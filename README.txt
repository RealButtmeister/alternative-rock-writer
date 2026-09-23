ALTERNATIVE ROCK WRITER

For the packaged edition, double-click Alternative Rock Writer.exe.
For the source edition, double-click Launch Alternative Rock Writer.vbs.
Keep that launcher, alt_rock_writer.py, lyric_engine.py, and song_structure.py
together. The source edition requires Python 3 with Tkinter; no extra Python
packages are needed.

GET STARTED
1. The app detects your existing OPENAI_API_KEY. Connection lets you enter
   another key for the current session or choose a different model.
2. Describe a conflict, a person, or a moment you cannot shake. Add real
   objects, places, textures, and words you would actually say.
3. The defaults focus on raw 1990s grunge and angst: short, spacious lines,
   an angry / worn-down voice, quiet-to-explosive dynamics, and concrete,
   uneasy imagery. Choose a different sound, mood, phrasing, rhyme approach,
   dynamics, or imagery when you want a different direction.
4. Add an optional title or chorus phrase. Use BLOCKED WORDS for entries
   that must stay out; use GOOD WORDS for ideas you like, with Require all
   enabled only when every entry must appear. Separate entries with commas
   or newlines.
5. Choose a length, or use Song structure to arrange sections and set lyric
   line counts. Write a song, then use Rewrite with a clear change request.
   Undo restores the previous version after a rewrite. Copy or Save .txt
   keeps your result. Save .txt opens a Save As file picker.

SONG JSON
Load song JSON accepts Song Structure.json from your MIDI arrangement.
The imported map keeps musical bars separate from lyric-line counts and
preserves section order, timing, and instrumental sections. Song structure
lets you review the imported map and edit lyric-line targets for vocal
sections. Clear imported song map returns to the manual arrangement controls.
The imported map and edited targets are saved with this app's preferences.

HOW IT WORKS
This is a separate alternative-rock edition of the latest Pop Indie Writer,
including its Song JSON import and validation. It drafts and revises original
lyrics using broad alternative-rock traits: tension, contradiction, physical
detail, rough edges, repeated hooks, and space for a loud chorus. It does not
copy an existing song or claim to reproduce any particular artist.

A generation normally uses two paid API requests, with up to four if checks
need repair. Blocked entries use case-insensitive whole-word or phrase
matching and Unicode normalization. A blocked word inside a longer word
does not match; add variants separately, such as "wire" and "wires".
Required good words, section order, and lyric-line counts are checked before
a generated result is shown. Copy and Save recheck the word rules and any
imported Song JSON map. Manual arrangements and preset line counts are
checked during generation, so review those counts after editing the draft.
Failed checks show the problem.
Chorus repetition, rhyme, imagery, and dynamics guide the writing rather
than imposing strict local checks. Sing the draft aloud and adjust it to
your tune. The app writes lyrics, not recordings or melodies.

CONNECTION AND SAVING
The default model remains GPT-5.5, matching the latest Pop Indie Writer.
Connection lets you change it. Generation requires internet access and an
OpenAI API key. API usage is billed separately from a ChatGPT subscription.
Your brief, word lists, song structure, and any lyrics submitted for rewriting
are sent to OpenAI to generate the result.

This edition starts with fresh settings and an empty song brief. Preferences
include your brief, word lists, controls, and imported song map. When running
the Python script, they are saved beside it. A packaged executable saves
them in Documents\Alternative Rock Writer. Neither shares Pop Indie Writer's
settings.
API keys entered in Connection stay in memory for the session and are never
saved to settings. Lyrics are saved only when you choose Save .txt.

Note on the fork
----------------
The original project seems abandoned, the fork at `dtantsur/mdx-video` adds
support for python-markdown 3+ and Python 3.12+.

Usage
-------
```python
import markdown

text = '...'
# see http://pythonhosted.org//Markdown/reference.html#extension_configs for passing parameters
html = markdown.markdown(text, extensions=['video'])
# or
from mdx_video import VideoExtension
html = markdown.markdown(text, extensions=[VideoExtension(**params)])
# or
md = markdown.Markdown()
md.registerExtension(VideoExtension(**params))
```

Support
-------

The following video providers are supported:

 - YouTube
 - Vimeo
 - Yahoo Video
 - Dailymotion
 - Metacafe
 - Veoh

Contribute
----------
Missed some provider?
Don't be shy, fork it and send a pull request.
Or you can open an issue too!

# blender-colab

<a href="https://colab.research.google.com/github/crimson-aril/blender-colab/blob/master/blender_render.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

This is a Python script that allows you to render Blender 5.0+ and older version scene using Google Colaboratory.
You can upload the blender files using direct upload, Google Drive or URL. Rendered frames can be downloaded directly or through Google Drive.
This script provides basic functionality so you may modify the script to your liking to suit your needs.

## Usage
### Upload type
* `direct`: Upload your blender file in the next cell.
* `google_drive`: The blender file will be downloaded directly from Google Drive. You need to specify the path to the blender/zip file at `drive_path`.
* `url`: Direct link to the blender file in `url_blend`.
* `gdrive_relative`: The Google Drive folder specified at drive_path will be copied directly (as if it's a zipped file).

### Download type
* `direct`: Output files will be automatically downloaded in your browser. (Probably does not work with multiple files?)
* `google_drive`: The output files will be pasted into the specified `drive_output_path` once rendering is finished.
* `gdrive_relative`: The output frames will be automatically rendered into the specified `drive_output_path`.

### A few notes
1. You must own a Google account.
2. One notebook can only run for maximum time of 12 hours (24 hours for Google Colab Pro) but not guaranteed.
3. EEVEE rendering is not supported in a virtual machine.
4. This script is not tested fully yet. Expect some errors.
5. Do note that your access to GPU may be limited or blocked if you render for many hours.
6. This script is intended for those who have no access to high-end GPU for rendering. Please use them responsibly!

## FAQ
### An error occured!
Check which section of the code failed and identify the error (such as misspelled files or path). If you don't understand the error, try re-running the code with the play button at the side. If it still fails, go to `Runtime > Restart and run all` to restart the code or try `Runtime > Factory reset runtime`. If all else fails, open an issue in GitHub with the error log you encountered attached and the details of your setup.

Common errors:
* `MessageError: TypeError: Failed to fetch` while downloading: The tab must be opened so that the frames can be downloaded.

## Disclaimer
Google Colab is targeted to researchers and students to run AI/ML tasks, data analysis and education, not rendering 3D scenes. Because the computing power provided are free, the usage limits, idle timeouts and speed of the rendering may varies time by time. [Colab Pro and Colab Pro+](https://colab.research.google.com/signup) are available for those who wanted to have more powerful GPU and longer runtimes for rendering. See the [FAQ](https://research.google.com/colaboratory/faq.html) for more info. In some cases, it might be faster to use an online Blender renderfarm.



## Licensing

This project is a combined and heavily modified work distributed under the terms of the GNU General Public License v3.0. 

### Original Work & Attribution
This project includes code originally authored by **syn73**, which is licensed under the MIT License:

---

MIT License

Copyright (c) 2020 syn73

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---

### Modifications & Derivative Code
All subsequent modifications, additions, and derivative works made to this project are:
**Copyright (c) 2026 Mohammed F. R. Noor (crimson-aril)**

The entire combined work is distributed under the terms of the GNU General Public License v3.0. You can review the full license terms in the accompanying `LICENSE` file or at <https://gnu.org>.


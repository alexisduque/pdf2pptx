# pdf2pptx
Convert your (Beamer) PDF slides to (Powerpoint) PPTX

So you dont like using Powerpoint and would rather use Latex/Beamer to make your slides,
however, you have a fancy Surface and you want to use the pen during the presentation? Here is my solution.

This script gets a PDF file as input and generates a Powerpoint PPTX file while preserving the format of the original PDF. Theoretically all PDF files, regardless of the original generator, can be converted to PDF slides with this (not tested though).

Simply explained, I convert all the slides to high-quality image files first, and then push them into a Powerpoint project as a slide.

# How to run
* Copy your pdf file next to the script first.
* Execute `./pdf2pptx.sh test.pdf` to generate a `test.pdf.pptx` file  (replace `test.pdf` with your filename).
* By default the output powerpoint project is in the widescreen mode. If your slides are not for widescreen you can alternatively run `./pdf2pptx.sh test.pdf notwide` to generate a 4:3 standard PPTX project.

# Dependencies
* You need `convert` from [ImageMagick] (http://www.imagemagick.org/script/binary-releases.php)
* `zip` and `sed`

If you're using Linux you *probably* already have all the above. If you're using OSX you need to install ImageMagick and make sure `convert` is accessible from your Terminal.

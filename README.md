# Auto-Make-Deliver-Report
Just because of my laziness

#### I. Environment
-- Ubuntu 14.01 <br>
-- Mozilla Firefox 43.0.4

#### II. Installation
Install Xvfb – The X Virtual FrameBuffer (Need to run with selenium)

  `$ sudo apt-get install xvfb`

Install selenium - Need to get HTML of JS page. Because gerrit use JS to generate HTML.

  `$ sudo pip install -U selenium`

Install reportlab - A Python lib allow to work with PDF file.

  `$ sudo pip install -U reportlab`


#### III. How to use
1. Copy and paste your gerrit links to <b>input.txt</b> file.

2. Edit <b>FIREFOX_BIN</b> in <b>deliver.py</b> file to your firefox dir. <br>
Show this dir with

  `$ which firefox`

3. Edit some configurations on <b>txt2pdf.py</b> if you want.

4. Get your deliver

  `$ xvfb-run python deliver.py`

5. Follow screen to make sure you don't miss anything.
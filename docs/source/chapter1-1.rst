chapter 1: minecraft
======================================

1.1  All tech books
-----------------------------

http://www.allitebooks.com/

모든 기술 서적은 상기 사이트에서 찾을 수 있음.


Beginning Blockchain
Bitcoin Essentials
Bitcoin For Dummies
Bitcoin for the Befuddled
Building Games with Ethereum Smart Contracts
Decentralized Applications
Mastering Bitcoin, 2nd Edition


1.1  minecraft+scratch
-----------------------------

https://github.com/mpatrascu/ScratchMC

ScriptCraft
~~~~~~~~~~~~~~~

https://github.com/walterhiggins/ScriptCraft/tree/master


https://github.com/tclavier/docker-scriptcraft


1.2  Scratch 3.0
-----------------------------


github
~~~~~~~~~~~~~~~

https://github.com/LLK/scratch-gui


electron
~~~~~~~~~~~~~~~

npm install -g asar

asar pack app app.asar

asar extract app.asar destfolder


scratch extension
~~~~~~~~~~~~~~~~~~~~~~
https://scratch.mit.edu/discuss/topic/289503/

node_modules\scratch-blocks

npm install

npm link

You can also use the command python build.py to build scratch blocks, but from my experience, changes aren't reflected
in the GUI unless you run npm link.


https://github.com/larjohn/rpi-scratch3-mqtt

https://github.com/larjohn/python3-pigpio-scratch3-mqtt



scratch-gui\node_modules\scratch-blocks\blocks_vertical
extensions.js
default_toolbox.js


scratch-gui\node_modules\scratch-blocks\media\extensions
seanpen-block-icon.svg 추가

scratch-gui\node_modules\scratch-blocks\i18n

scratch-gui\node_modules\scratch-l10n\scripts
build-data.js
build-i18n-src.js

scratch-gui\node_modules\scratch-vm\src\extensions

scratch3_seanpen
index.js
Scratch3PenSEANBlocks 변경

scratch-gui\node_modules\scratch-vm\src\extension-support

extension-manager.js
const Scratch3PenSEANBlocks = require('../extensions/scratch3_seanpen');

const builtinExtensions = {
    pen: Scratch3PenBlocks,
    seanpen: Scratch3PenSEANBlocks,
    wedo2: Scratch3WeDo2Blocks,
    music: Scratch3MusicBlocks,
    microbit: Scratch3MicroBitBlocks,
    text2speech: Scratch3Text2SpeechBlocks,
    translate: Scratch3TranslateBlocks,
    videoSensing: Scratch3VideoSensingBlocks,
    speech2text: Scratch3Speech2TextBlocks,
    ev3: Scratch3Ev3Blocks
};

scratch-gui\src\lib\libraries\extensions

index.jsx

import seanpenImage from './seanpen.png';
import seanpenInsetImage from './seanpen-small.svg';

cratch-gui\src\lib\libraries\extensions 이미지 등록


scratch-gui\translations\messages\src\lib\libraries\extensions
index.json


mblock bluetooth
~~~~~~~~~~~~~~~~~~~~~~~~

https://github.com/inker610566/MBlocky
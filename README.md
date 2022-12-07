#The Pronounce

A command line interface for English words pronunciation.

This program retrieves pronunciation files from the [dictionary.com]
(https://www.dictionary.com/) website, which are publicly available
to be downloaded and plays them automatically.
This command downloads the pronunciation OGG files via [wget](http://www.gnu.org/software/wget/), stores them
locally in the **~/.cache/pronunciation.ogg** folder, and plays them via [ffplay](http://ffmpeg.org/ffplay.html).

##Installation

1. Copy the _pronounce_ script somewhere in your path, for example in
the **/usr/bin** folder.
2. Create the **~/.cache/pronunciation.ogg** folder.
3. And install the [ffplay](http://ffmpeg.org/ffplay.html) (usually comes with the _ffmpeg_ package).

##Usage

You can run pronounce in 4 modes.

 * Mode 1: _pronounce <word>_

   To listen to default pronunciation of a word, e.g. _live_, as found on the Web, type:

        pronounce live

 * Mode 2: _pronounce <word> <number>_

   To listen to the _i-th_ available pronunciation of a word, e.g. the 2nd pronunciation of _live_ (which has different pronunciations as noun and verb), type:

        pronounce live 2
  
 * Mode 3: _pronounce <word> f_

   To open the given word's definition page, e.g. _live_, in [firefox](http://www.firefox.com/), type:

        pronounce live f
  
   This mode, internally runs the following command:

        firefox "https://www.dictionary.com/browse/live"

 * Mode 4: _pronounce <word> w_

   To open the given word's definition page, e.g. _live_, in [w3m](http://w3m.sourceforge.net/) command line browser, type:

        pronounce live w

   This mode, internally runs the following command:

        w3m "https://www.dictionary.com/browse/live"

##License
    Copyright © 2013-2022  Behnam Momeni

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see {http://www.gnu.org/licenses/}.


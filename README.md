datacoin
========
http://datacoin.info

https://datacointalk.org

Copyright (c) 2013 Primecoin Developers

Copyright (c) 2009-2013 Bitcoin Developers

Copyright (c) 2011-2013 PPCoin Developers

Copyright (c) 2014 Datacoin developers

### What is Datacoin?
Datacoin is a reliable, censorship-free currency that can be used for transactions and data storage within its sophisticated blockchain.

Data is stored in the blockchain forever and can be retrieved using a transaction hash as an identifier. Datacoin is a platform that can be used by applications such as torrent trackers, encrypted messaging services, and can be used to store other kinds of small data - all censorship-free!

Developers can store torrent files, certificates, and with future development, HTML pages and other kinds of meta-information in the Datacoin blockchain.

You can install the wallet from the right-side menu. Windows users can use a GUI wallet, Linux users should compile datacoind or Datacoin-QT from source (see instructions). Wallets are in development, and more features are coming soon, but the wallet's current functionality is similar to other coins.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Datacoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion (if they haven't already) on the
ppcoin/primecoin forum (http://datacointalk.org).

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/switchpwn/datacoin/tags) are
created regularly to indicate new official, stable release versions of
Primecoin.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test datacoin-qt.pro
    make -f Makefile.test
    ./datacoin-qt_test

### Manual Quality Assurance (QA) Testing

Large changes should have a test plan, and should be tested by somebody other
than the developer who wrote the code.

See https://github.com/bitcoin/QA/ for how to create a test plan.

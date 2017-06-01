dragvisuals
===========

This is **exact** copy of `Damian Conway`_ script for moving visually selected
blocks around. The purpose of this repository is to make it more convenient for
package managers like Pathogen_.

Installation
------------

To install it, any kind of Vim package manager can be used, like NeoBundle_,
Pathogen_, Vundle_ or vim-plug_.

For manual installation, copy subdirectories from this repository to your
``~/.vim`` directory.

Usage
-----

To use it, add the following  to your ``.vimrc``:

.. code:: vim

   vmap  <expr>  <LEFT>   DVB_Drag('left')
   vmap  <expr>  <RIGHT>  DVB_Drag('right')
   vmap  <expr>  <DOWN>   DVB_Drag('down')
   vmap  <expr>  <UP>     DVB_Drag('up')
   vmap  <expr>  D        DVB_Duplicate()

   " Remove any introduced trailing whitespace after moving...
   let g:DVB_TrimWS = 1

Or, if you use the arrow keys for normal motions, choose four other keys for
block dragging. For example:

.. code:: vim

   vmap  <expr>  h        DVB_Drag('left')
   vmap  <expr>  l        DVB_Drag('right')
   vmap  <expr>  j        DVB_Drag('down')
   vmap  <expr>  k        DVB_Drag('up')

Or:

.. code:: vim

   vmap  <expr>  <S-LEFT>   DVB_Drag('left')
   vmap  <expr>  <S-RIGHT>  DVB_Drag('right')
   vmap  <expr>  <S-DOWN>   DVB_Drag('down')
   vmap  <expr>  <S-UP>     DVB_Drag('up')

Or even:

.. code:: vim

   vmap  <expr>   <LEFT><LEFT>   DVB_Drag('left')
   vmap  <expr>  <RIGHT><RIGHT>  DVB_Drag('right')
   vmap  <expr>   <DOWN><DOWN>   DVB_Drag('down')
   vmap  <expr>     <UP><UP>     DVB_Drag('up')

License
-------

This work is placed under public domain.

.. _Pathogen: https://github.com/tpope/vim-pathogen
.. _Vundle: https://github.com/gmarik/Vundle.vim
.. _NeoBundle: https://github.com/Shougo/neobundle.vim
.. _vim-plug: https://github.com/junegunn/vim-plug
.. _Damian Conway: https://github.com/thoughtstream/Damian-Conway-s-Vim-Setup

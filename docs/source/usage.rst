Usage
=====

.. _warning:

Warning
------------

The collection while it has a few customizable options is **NOT** designed to be modified. The smallest change ***as simple as changing pocket size*** has caused game breaking issues and profile loss. Because of this I will provide **ZERO** support for anyone who modifies the collection even the slightest and feedback will not be taken into consideration.

Those who alter the collection in any way and are discovered to have done so ***while still asking for help and/or lying*** about modifying the collection will be **permanently banned** from the discord. I put a lot of time into this collection and don't enjoy being taken advantage of or my free time being wasted. This collection is free, and I would like my time and person to be respected.


Keep in mind that a lot of these mods are altered **minimally to significantly** and do not function as they would normally due to this but function as I intend them to.

For now **DO NOT** build/upgrade both ***Med station & Water collector***. You can have **ONE** or the other but not both. This is due to an error thrown the breaks the game because of it. This is a priority one issue, but I have no idea when I will fix it. I suggest not building Water Collector but you are free to choose. This is an issue left behind from the previous mod author of Traveler in said mod which is now Wayferer and has significant changes made to it's locations, new ones added, etc.

**ALWAYS KEEP A BACK UP OF THE PREVIOUS GAME VERSION IN CASE YOU RUN INTO ERRORS/ISSUES IN THE NEW RELEASES**

.. _requirements:

:::{Requirements}
:class: dropdown

Requirements
------------

``.Net 6 Desktop Runtime`` 
https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-6.0.4-windows-x64-installer

A **legitimate** copy of Escape From Tarkov.
Do NOT use WinRAR; it is known to cause issues. Use ``7Zip``

:::


.. _how to setup:

How to Setup
------------

1. Create a Beyond The Borders - Legacy Edition (3.7.6.) folder for use during installation/set-up (Must be created on your C:Drive).
2. Install SPT (Single Player Tarkov) correctly in the created Beyond The Borders - Legacy Edition (3.7.6.) folder:  https://hub.sp-tarkov.com/files/file/672-spt-installer/
Make sure to run the server & launcher at once before the next steps. Do not create a profile or copy live tarkov settings. Then close out of both server and launcher
3. Delete all the folders except for ``EscapeFromTarkov_Data`` , ``EscapeFromTarkov.exe``, ``EscapeFromTarkov_BE.exe``
4. Extract patcher (BtB-Patcher-3.7.6.7z) with 7zip ONLY into a separate folder. Patcher Link: https://drive.google.com/file/d/10mXnFqAa-ktwFD64DWNU34ScWxUZ68I6/view?usp=sharing
5. Copy the files inside the BtB-Patcher-3.7.6.7z newly extracted folder into the Beyond The Borders - Legacy Edition (3.7.6.) folder.
6. Run the patcher.exe that is now inside the Beyond The Borders - Legacy Edition (3.7.6.) folder.
7. Once it has finished, delete the ``patcher.exe``.



.. _installation:

Installation
------------

To use Lumache, first install it using pip:

.. code-block:: console

   (.venv) $ pip install lumache

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']


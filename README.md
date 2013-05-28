nsisXML
=======

Modification of the nsisXML plugin (by Wizou)

Added setNamespace method to work with selecting nodes inside of a namespace.

Example xml of why this was needed.

<?xml version="1.0" encoding="UTF-8"?>

\<main xmlns="namespace">

  \<child>content\</child>
  
\</main>

The existing code could not find the correct node when searching for /main/child.

Usage:
  nsisXML::setNamespace "xmlns:a='namespace'"
  nsisXML::select "/a:main/a:child"

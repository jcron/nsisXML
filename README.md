nsisXML
=======

Modification of the nsisXML plugin (by Wizou)

Added setNamespace method to work with selecting nodes inside of a namespace.

See Sample.xml for an example of why this was needed.

Usage:
  nsisXML::setNamespace "xmlns:a='namespace'"
  nsisXML::select "/a:main/a:child"

Changelog
=========


1.4 (unreleased)
----------------

- Nothing changed yet.


1.3 (2016-09-21)
----------------

- Feature: only export fields where the current user has the permission to read
  that field. The security check doesn't not happen on the object but
  on the context of the calling view for performance reasons.
  [pcdummy]

- Fix: try to get the value of a method if the field is a method and translate
  DateTime results to a unicode, this fixes the export for objects with the IPublication
  Behavior.
  [pcdummy]

- Fix: be sure to not retrieve an attribute on an object by acquisition.
  [vincentfretin]

- Feature: render_style can now return a Style object with content and headers
  attribute to be able to customise the header style per exportable.
  [vincentfretin]

- Feature: the passed obj to render_value is now
  exportable.field.bind(obj).context to make it easier to get data from
  parent or grandparent.
  [vincentfretin]

- Feature: BaseFieldRenderer.render_header method returns now the translated field
  title instead of the Message object.
  [vincentfretin]

- Fix: Ignore reverse parameter when creating export url.
  [cedricmessiant]

- Feature: Add sort exportables feature using exportables_order list.
  [cedricmessiant]

- Fix: Sort exportables features even if they are not fields
  [ebrehault]


1.2 (2014-09-10)
----------------

- Feature: Added export under csv format.
  [thomasdesvenain]

- API: Filter exportables by field name by default using excluded_exportables list.
  [cedricmessiant]

- API: We can define a dexterity adapter for just one field using field name as
  adapter name.
  [thomasdesvenain]

- Fix: Faceted nav export link ignores results per page criterion.
  [thomasdesvenain]

- Fix: Translate sheet title.
  [thomasdesvenain]

- Fix: Improve text fields support.
  [fngaha, thomasdesvenain]

1.1 (2014-06-19)
----------------

- Rename search policy excelexport.search to avoid conflict with 'search' view.
  [thomasdesvenain]


1.0 (2014-06-02)
----------------

- Initial release.
  [thomasdesvenain]

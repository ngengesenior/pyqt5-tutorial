Wizard
======
A Wizard is a helper widget which allows for paginated display of information which the user can progress through. They are commonly used for setup of new programs or building up information prior to an action.

===========
Constructor
===========
The Wizard is constructed with the statement::

  wizard = QWizard()

=======
Methods
=======
A page can be added to the Wizard via the two methods::

  wizard.addPage(page)
  wizard.setPage(number, page)

The *page* parameter should be the :doc:`wizardpage` object which is to be added. The *number* indicates the position at which the page should be added.

Pages can also be removed by specifying the page number::

  wizard.removePage(number)

The title used on the page can be set with::

  wizard.setTitle(title)

The page object for a given page number can be retrieved using::

  wizard.page(number)

The current page object and number can be retrieved with the calls::

  wizard.currentPage()
  wizard.currentId()

A check can be made on whether a user has visited a particular page via::

  wizard.hasVisitedPage(number)

Alternatively, a list of visited pages can be obtained in list form with::

  wizard.visitedPages()

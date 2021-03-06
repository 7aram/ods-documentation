Configuring a dataset for calendar view
=======================================

The OpenDataSoft platform lets you easily create calendar views from your published datasets.

.. ifconfig:: language == 'en'

    .. figure:: calendar__result--en.png

       A calendar built from a dataset containing all events from OpenAgenda

.. ifconfig:: language == 'fr'

    .. figure:: calendar__result--fr.png

       A calendar built from a dataset containing all events from OpenAgenda

Datasets requirements
---------------------

For the calendar view, each record of your dataset is a different event. These events must contain a start time, an end 
time and a title. Which means your dataset must have two datetime fields and a text field for the calendar view to be 
available.

.. ifconfig:: language == 'en'

    .. figure:: calendar__processing_settings--en.png

       2 fields set as datetime

.. ifconfig:: language == 'fr'

    .. figure:: calendar__processing_settings--fr.png

       2 fields set as datetime

Records without titles will be displayed on the calendar as titleless events, but missing either the start or end time 
will cause the view to simply ignore the record.

Full day events
~~~~~~~~~~~~~~~

Though very simple, the "two datetime fields and a text field" requirement forces you to setup full day events as events ~
starting at 12AM on the given day and finishing a second before midnight on the same day (00:00:00 to 23:59:59).

Configuration
-------------

Enabling the calendar view
~~~~~~~~~~~~~~~~~~~~~~~~~~

Once you have configured two of your dataset's fields as datetimes and another field as text, you'll see the calendar 
tab become available.

.. ifconfig:: language == 'en'

    .. figure:: calendar__tab_unavailable--en.png

       Calendar tab unavailable

    .. figure:: calendar__tab_available--en.png

       Calendar tab available

.. ifconfig:: language == 'fr'

    .. figure:: calendar__tab_unavailable--fr.png

       Calendar tab unavailable

    .. figure:: calendar__tab_available--fr.png

       Calendar tab available

It doesn't mean that your dataset is fully configured though. The view is available but not enabled by default. You'll 
have to manually enable it.

.. ifconfig:: language == 'en'

    .. figure:: calendar__checkbox--en.png

       This checkbox will enable the calendar view

.. ifconfig:: language == 'fr'

    .. figure:: calendar__checkbox--fr.png

       This checkbox will enable the calendar view

Setting up events' fields
~~~~~~~~~~~~~~~~~~~~~~~~~

Once the calendar is enabled, you'll need to make sure the events' fields are well configured. You'll see that the first
text field has been selected for the title, the first datetime for the start time and the second datetime for the end 
time. You may have multiple other text/datetime fields in your dataset, select here which one determine the events' 
properties.

This is also where you'll be able to select the events' color.

.. ifconfig:: language == 'en'

    .. figure:: calendar__event_default_settings--en.png

       Default configuration for my calendar. The event's fields are pre-selected but not correct.

    .. figure:: calendar__event_settings--en.png

       Corrected settings

.. ifconfig:: language == 'fr'

    .. figure:: calendar__event_default_settings--fr.png

       Default configuration for my calendar. The event's fields are pre-selected but not correct.

    .. figure:: calendar__event_settings--fr.png

       Corrected settings

Setting up the tooltip
~~~~~~~~~~~~~~~~~~~~~~

In the calendar view, a click on a event will bring forward a tooltip containing more information about the events. You 
can of course configure which fields will appear in the tooltip and their relative order. A live preview is available 
on the right side.

.. ifconfig:: language == 'en'

    .. figure:: calendar__tooltip_settings--en.png

       Setting up the tooltip

.. ifconfig:: language == 'fr'

    .. figure:: calendar__tooltip_settings--fr.png

       Setting up the tooltip

For each of the tooltip's fields, the 3 following actions are available :

.. figure:: calendar__tooltip_actions.png

   Tooltip's fields' actions

* Drag and drop to move field within tooltip
* Click to remove field from tooltip
* Click to add field to tooltip

.. ifconfig:: language == 'en'

    .. figure:: calendar__tooltip_preview--en.png

       The associated live preview

.. ifconfig:: language == 'fr'

    .. figure:: calendar__tooltip_preview--fr.png

       The associated live preview

Sharing
-------

Once your dataset is correctly setup and published, you can of course share this calendar with anyone having the rights 
to view the calendar.

To do so, you can always copy/paste the url from your browser's address bar, but you can also use any of the 3 options 
offered below the calendar itself.

1. Share the url

.. ifconfig:: language == 'en'

    .. figure:: calendar__share--en.png

       The 3 sharing options, with first and foremost the url

.. ifconfig:: language == 'fr'

    .. figure:: calendar__share--fr.png

       The 3 sharing options, with first and foremost the url

2. Code snippet to embed the view inside any other website

.. ifconfig:: language == 'en'

    .. figure:: calendar__embed--en.png

       Embed this code into any other page to display your calendar there

.. ifconfig:: language == 'fr'

    .. figure:: calendar__embed--fr.png

       Embed this code into any other page to display your calendar there

3. Code snippet to include in any of your dashboard or page on the platform.

.. ifconfig:: language == 'en'

    .. figure:: calendar__widget--en.png

       Copy this code to one your dashboard on the platform

.. ifconfig:: language == 'fr'

    .. figure:: calendar__widget--fr.png

       Copy this code to one your dashboard on the platform

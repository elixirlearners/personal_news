# Personal News
An Elixir project that generates a periodical with information relevant to its owner.

The design is inpsired by a newspaper from an aesthetic and information
heirarchy point of view. "Editions" will be delivered at appropriate times as
desired.

Initially layout will be fairly static/hardcoded, but as the information
content grows a dynamic rendering mode will be added that shows the most
important information at the top and queues less important information for
later on (or page 2, etc). ML will be used to expand or shrink content to fit
the appropriate sizes.

A system of plugins will support information gathering both via pulling
directly from available sources and jobs that push data in at various times.

Some examples of plugin support desired:
 - Home Assistant (and other home automation integrations)
 - Server management (keep track of status/health/backups/security/etc)
 - Email (inbound analysis/important items/parsing)
 - Web scraping/Searches (specific sites for relevant updates)
 - Account updates (check for messages, notifications, etc)
 - Baby monitor (app)
 - Extensible so more can be added easily

Views/Rendering modes:
 - Web view
 - E-Ink View (optimized for B&W + target resolutions)
 - Email (newsletter style)
 - Printout (letter sized, thermal?)

Each edition should store the relevant rendering information so that it can be
recreated at later points (to view an archive the same way it was originally
created).

A first step will to be developing one or two plugins and rendering some
details from them in a livebook.

Not determined:
 - Whether the views will be fully static, or allow interaction.
 - How the onboarding flow should work (eventually this should be a hosted app
   that can support enrollment by non-Elixir devs)

Example/mockup:
![mockup-personal-news](https://github.com/elixirlearners/personal_news/assets/1295934/f0261daf-ceb7-489c-94cc-3cb680b81f5c)



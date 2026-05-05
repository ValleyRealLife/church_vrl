# Plugins for Valley Real Life

This repository contains the plugins built and used by Valley Real Life in Rock RMS. The files are stored in church_vrl on the dev and production servers.

## FlexiContentComponents

This is a custom block that was cloned from the core WebForms content component block. The purpose was to create a solution that allows for the selection of specific content channel types to prevent the pollution of the block properties attributes with irrelevant attributes depending on the context.

The OG core block is hard coded to "CONTENT_COMPONENT" as a singular content channel type. So any attributes there are global across all contexts (sites, pages, everywhere).

This solution adds a simple dropdown on the block properties that allows the user to select which Content Channel Type should be used for that particular block. This will populate that content channel with the contextualized item and channel attributes.

It also exposes the start and expire dates of the content channel item to the block which was necessary for the project I was working on. In theory, any content channel item property could be exposed.

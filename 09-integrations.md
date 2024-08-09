---
title: Integrations
teaching: 10
exercises: 0
---

::::::::::::::::::::::::::::::::::::::: objectives

- Explain what integrations are
- Explain how integrations support advanced record actions

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- What are integrations?
- What work can integrations support?

::::::::::::::::::::::::::::::::::::::::::::::::::

## Integrations

MarcEdit has the ability to interface (or integrate) with other applications. Integrations with other cataloguing utilities, such as vendor ILS and LSP systems and OCLC WorldCat, support advanced actions which can include downloading records, pushing new records or record updates, and setting holdings (OCLC WorldCat). Currently, MarcEdit can integrate with the ILS Alma, Koha, or a local ILS if you are able to connect to the host database. MarcEdit can be set up to integrate with OCLC's APIs for metadata and connect to OCLC or the Library of Congress (either UTF-8 or MARC8) Z39.50 services.

For the ILS integrations you will need one or some of the following:

- Host URL of the database
- Username and password
- Token

If you are setting up an integration to your ILS, it is recommended to touch base with those who have already done this. For example, for Alma, you can reach out to the Alma listserv to get guidance.

For the OCLC API integration, you will need to request an API key with OCLC. You will need the Registry API, Metadata API, and Search API. It is recommended to consult OCLC's help page on [setting up MarcEdit OCLC integration](https://help.oclc.org/Librarian_Toolbox/OCLC_APIs/Troubleshooting/How_do_I_set_up_MarcEdit_OCLC_Integration%3F?sl=en) as well as Terry Reese's information from his blog.

For the Z39.50 integration, you will need to enter your username and password in the settings. For OCLC, this is your Connexion number and password. For the Z39.50 search for OCLC, there are options for the types of searches performed and translating records to UTF-8.

:::::::::::::::::::::::::::::::::::::::: keypoints

- Understand what integrations are and why they're useful
- Understand where to set up an integration

::::::::::::::::::::::::::::::::::::::::::::::::::



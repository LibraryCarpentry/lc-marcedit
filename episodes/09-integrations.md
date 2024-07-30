---
title: Integrations
teaching: 15
exercises: 0
---

::::::::::::::::::::::::::::::::::::::: objectives

- Explain what integrations are
- Explain how integrations support advanced record actions
- Illustrate integrations with OCLC

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- What are integrations?
- What work can integrations support?

::::::::::::::::::::::::::::::::::::::::::::::::::

## Integrations

MarcEdit can interface (or integrate) with other applications. Integrations with other cataloguing utilities, such as vendor ILS and LSP systems and OCLC WorldCat, support advanced actions, including downloading records, pushing new records or record updates, and setting holdings (OCLC WorldCat). Currently, MarcEdit can integrate with the ILS Alma, Koha, or a local ILS if you can connect to the host database. MarcEdit can be set up to integrate with OCLC's APIs for metadata and connect to OCLC or the Library of Congress (UTF-8 or MARC8) Z39.50 services.

For the ILS integrations you will need one or some of the following:

- Host URL of the database
- Username and password
- OCLC Connexion username and password
- Token
- API Key

### Integration with an ILS
At this time, MarcEdit supports integrations with the ILS Alma and Koha. The ILS integration will require you to request an API key from your systems person, your ILS vendor, or your hosting vendor. You can also ask for instructions on how to set up the integration. For example, for Alma, you can reach out to the Alma listserv to get guidance or to the Alma Tech Blog on [integrating MarcEdit with Alma](https://developers.exlibrisgroup.com/blog/configure-marcedit-7-to-work-with-alma-updated-for-marcedit-7-5-116-12-17-2021/). For Koha, this [article](https://bywatersolutions.com/education/koha-tutorial-exporting-records-marcedit) from ByWater Solutions offers guidance on how to edit records in MarcEdit using the Koha MarcEdit integration.

### Integration with OCLC's API
For the OCLC API integration, you need to [request an API key and check if your institution is eligible](https://www.oclc.org/developer/support/eligibility.en.html) for this service. If your institution is eligible, then you can request a key through [OCLC's developer network](tps://www.oclc.org/developer/develop/authentication/how-to-request-a-wskey.en.html). You can also go to Preferences from the main menu in MarcEdit, click on OCLC API Integration and then click on the "Request an OCLC Key". It is recommended to consult OCLC's help page on [setting up MarcEdit OCLC integration]([https://help.oclc.org/Librarian_Toolbox/OCLC_APIs/Troubleshooting/How_do_I_set_up_MarcEdit_OCLC_Integration%3F?sl=en](https://help.oclc.org/Librarian_Toolbox/OCLC_APIs/Troubleshooting/How_do_I_set_up_MarcEdit_OCLC_Integration%3F)) as well as Terry Reese's information from his blog.

### Integration with a Z39.50 Database
Many systems rely on the Z39.50 protocol. It could be the case that your current ILS relies on it for Interlibrary loan. For this type of integration, you need the following information below. You can find this information at the Library of Congress [Gateway to Library Catalogs](https://www.loc.gov/z3950/) of [zbrary](https://www.z-brary.com/).

<table>
  <tr>
    <td><strong>Field</strong></td>
    <td><strong>Value</strong></td>
  </tr>
  <tr>
    <td>Name</td>
    <td>Enter a name that helps you remember which Z39.50 service you are connecting to</td>
  </tr>
  <tr>
    <td>Host</td>
    <td>The link to the host's Z39.50.</td>
  </tr>
  <tr>
    <td>Database</td>
    <td>Enter the name of the database</td>
  </tr>
  <tr>
    <td>Port</td>
    <td>Enter the port number</td>
  </tr>
  <tr>
    <td>Syntax</td>
    <td>Enter the flavor of MARC such as USMARC</td>
  </tr>
  <tr>
    <td>Username</td>
    <td>Enter a username</td>
  </tr>
</table>

For [OCLC](https://help.oclc.org/Metadata_Services/Z3950_Cataloging/Get_started/Configuration_guide_for_OCLC_Z39.50_Cataloging), this information looks like the following. 

<table>
  <tr>
    <td><strong>Field</strong></td>
    <td><strong>Value</strong></td>
  </tr>
  <tr>
    <td>Name</td>
    <td>OCLC's Library Catalog</td>
  </tr>
  <tr>
    <td>Host</td>
    <td>zcat.oclc.org</td>
  </tr>
  <tr>
    <td>Database</td>
    <td>OLUCWorldCat</td>
  </tr>
  <tr>
    <td>Port</td>
    <td>210</td>
  </tr>
  <tr>
    <td>Syntax</td>
    <td>MARC21</td>
  </tr>
  <tr>
    <td>Username & Password</td>
    <td>Connexion Username of 3 numbers - 3 numbers - 3 numbers as in 100-034-090 and your Connexion Password</td>
  </tr>
</table>

You should be able to add multiple Z39.50 connections.

:::::::::::::::::::::::::::::::::::::::: keypoints

- Understand what integrations are and why they're useful
- Understand where to set up an integration

::::::::::::::::::::::::::::::::::::::::::::::::::



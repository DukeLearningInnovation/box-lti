# box-lti
Box LTI integration with Sakai

## Sakai Information
Sakai is an [Apereo Foundation](http://www.apereo.org) project and follows the Foundation's [guidelines and requirements for Contributor License Agreements](https://www.apereo.org/licensing).

Sakai is licensed under the [Educational Community License version 2.0](http://opensource.org/licenses/ECL-2.0)

Sakai's [Github wiki](https://github.com/sakaiproject/sakai/wiki) contains lots of useful links for getting started with development. 

Specifics about contributing to Sakai can be found in [sakai/CONTRIBUTING.md](https://github.com/sakaiproject/sakai/blob/master/CONTRIBUTING.md)

## Box Information


## LTI Information
The [Learning Tool Interoperability standard](https://www.imsglobal.org/activity/learning-tools-interoperability) is an open standard agreed upon by education institutions and vendors that serve them to integrate education technologies.

IMS Global, who maintains the LTI standard, has several repositories which may be useful for learning how to implement the standard.

* [basiclti-util-java](https://github.com/IMSGlobal/basiclti-util-java)
* [LTI-Tool-Provider-Library-PHP](https://github.com/IMSGlobal/LTI-Tool-Provider-Library-PHP)
* [LTI-Sample-Tool-Provider-PHP](https://github.com/IMSGlobal/LTI-Sample-Tool-Provider-PHP)

A LTI integration exists for Box and the Canvas LMS which may provide some technical guidance.

* [documentation](https://app.box.com/s/ib3bzr4nj2vl443wqxtm)
* [repository](https://github.com/instructure/lti-box-engine)

## What box-lti does


### Create a Box folder for a Sakai site

1. Sakai user with Admin, Instructor, TA, or Course Builder role in a site clicks Site info :: Manage Tools
1. From the list, click the checkmark next to Box
1. A LTI Launch is sent to box-lti
1. box-lti creates a Box folder using the data sent in the LTI Launch

This will add Box to the lefthand site navigation and enable further workflows below.

### Future
Possible next steps include:

* allow user to select whether to create a new folder or reusing an old Box folder. 

### Insert Box resource
Using the [LTI Deeplink spec](https://www.imsglobal.org/specs/lticiv1p0)

1. Sakai user in a site with Box enabled clicks anywhere that brings up the wysiwyg editor
![Sakai CK Editor](_assets/CKEditor.png)
1. User clicks the `InsertContentItem` icon, represented by a shopping cart in the image above
1. This brings up a list of compatible apps, user selects Box
1. A new window appears with the Box folder for the course shown, the user selects which content they desire and inserts a deep link to the content.

### Future
Possible next steps include:

* allow user to link or embed the file using the Box Viewer API


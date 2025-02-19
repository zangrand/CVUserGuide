..    include:: <isonum.txt>


Registration
============

To be able to use the CloudVeneto service, first of all you need to
apply for an account. The procedure to be followed is described in this
chapter.

Users who need to use INFN IT resources (i.e. users willing to be member of
an INFN project) must met the prerequisites specified in the following
section before applying for an account on the CloudVeneto infrastructure.

Prerequisites for using INFN resources
--------------------------------------
Users who need to use INFN IT resources must:

- have a verified digital identity (LoA2) on INFN-AAI;
- declare to have read and accepted the INFN rules for the use of IT resources;
- have followed the "Corso di Sicurezza Informatica - BASE".

To have a verified digital identity, connect to
https://signup.app.infn.it/ to self-register and to get an account on
INFN-AAI. Documentation (unfortunately only in Italian)
on this process is available `here <https://wiki.infn.it/cn/ccr/aai/doc/rid/istruzioni>`__.

After this self-registration process, connect to the INFN-AAI User Portal at
https://userportal.app.infn.it/ using your INFN-AAI account 
to complete the digital identity registration. In this process you will
have to choose where (the INFN site) you want to be identified, and
the person that will have to approve your request.
Documentation (unfortunately only in Italian) on this process
is available `here <https://wiki.infn.it/cn/ccr/aai/doc/rid/istruzioni>`__.

You will then be contacted by an INFN secretariat person for your identification.

To follow the "Corso di Sicurezza Informatica - BASE", please use
`this link <https://elearning.infn.it/course/view.php?id=105>`__.
**This course must be followed within 30 days after the registration.**


.. NOTE::

   These rules apply to users willing to be member of an INFN project, but 
   also
   to users who want to join a Physics Dept. related project using a
   10.64.x.0/24 network (since this is a INFN network).


Apply for an account
--------------------

The registration procedure in the cloud is managed through the Horizon
Openstack web service interface.

Go to https://cloud-areapd.pd.infn.it/dashboard or
https://cloudveneto.ict.unipd.it/dashboard in a browser. The following
page should appear:

.. image:: ./images/dashboard_prod.png
   :align: center

Click on the **Register** button. 

The following page should appear:

.. image:: ./images/dashboard_reg.png
   :align: center


-  If you have an account on the INFN Authenticaton and
   Authorization Infrastructure (INFN AAI) and therefore you have access
   to the INFN portal, click on the INFN AAI logo and proceed with :ref:`Enrollment procedure through INFN AAI or UniPD SSO<Enrollment>`.

-  If you instead have an account on the UniPD Single Sign-On (SSO)
   Infrastructure (e.g. you have a username @unipd.it or
   @studenti.unipd.it), click on the UniPD logo and proceed with :ref:`Enrollment procedure through INFN AAI or UniPD SSO<Enrollment>`.

-  If and only if you don't have neither an account on the INFN
   Authenticaton and Authorization Infrastructure (INFN AAI) nor on the
   UniPD SSO, click on the last icon (the green one, with "Username"
   and "Password") and proceed with :ref:`Apply for an account using User and Password<ApplyUsingUserPasswd>`.

Enrollment procedure through INFN AAI or UniPD SSO
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
.. _Enrollment:


Once authenticated on your Identity Provider system, you will be
redirected to a form like this:


.. image:: ./images/RegisterFormAAI.jpg 
   :align: center



Fill the form with the required information. In particular please specify 
the relevant unit/department of your home institution.

For what concerns the **Project Action** (projects have been discussed in 
:ref:`Projects<projects>`)
you have two options:

-  Select Existing Projects

-  Create new project

Choose **Select Existing Projects** if you want to apply membership for
one or more existing projects (choose them in the relevant box).

Select **Create new project** if instead you want to ask the creation of
a new project (and you are the leader of the experiment/research group
associated to this project). In this case you will have to specify also
a Project name and a Project Description. 

You will
also have to specify if this project must be private (a personal project
where you will be the only member) or not.


Newly created projects will get a default quota of:

-  20 VCPU

-  20 GB RAM

-  200 GB for Volume (e.g. non ephemeral) storage

Allocation of more resources for UniPD users must be approved by the
Cloud UniPD "governance". Mail your request to
cloud-unipd-gov@lists.pd.infn.it if you want more resources to be
allocated to your project.

.. NOTE::

    Public (i.e. not private) projects are projects where other users
    can apply for membership. They are supposed to be used for
    experiments or other research groups.

    **Personal private projects are discouraged** and are created only
    for convincing reasons.


.. NOTE::

    The person who asks for the creation of a new project is
    automatically defined as the manager of this project, i.e. he/she
    will have to manage the membership requests for this project. So the
    request to create a new project should be done by the relevant
    experiment/group leader.


When you have filled the form, please read the AUP that you need to
accept (by clicking the **Accept AUP** button).

Finally click on the **Register** button and you are done.


.. image:: ./images/RegistrationDone.png
   :align: center



Your request will be managed by the Cloud adminstrator and by the
manager(s) of the project(s) for which you applied membership. You will
get an e-mail when your request is approved or if for some reason your 
request is refused.
In the first case you will also receive an e-mail for the credentials
needed to access the Cloud gate machine (see :ref:`Network Access<NetworkAccess>`).


Apply for an account using Username and Password
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
.. _ApplyUsingUserPasswd:


If and only if you don't have an account on the UniPD SSO or INFN AAI,
click on the green icon on the right:

.. image:: ./images/RegisterLocalAccount.png
   :align: center


A form such as the one of the
following image will appear.

.. image:: ./images/RegisterFormUserPasswd.png
   :align: center



Please fill the form with your personal data (First Name, Last Name, Email
Address. 
Choose a User
name (please note that it could be changed by the Cloud admins during
the registration process) and a Password. 
Specify your home institution and the relevant unit/department.

For what concerns the **Project Action** (projects have been discussed in 
:ref:`Projects<projects>`)
you have two options:

-  Select Existing Projects

-  Create new project

Choose **Select Existing Projects** if you want to apply membership for
one or more existing projects (choose them in the relevant box).

Select **Create new project** if instead you want to ask the creation of
a new project (and you are the leader of the experiment/research group
associated to this project). In this case you will have to specify also
a Project name and a Project Description. 

You will
also have to specify if this project must be private (a personal project
where you will be the only member) or not.


Newly created projects will get a default quota of:

-  20 VCPU

-  20 GB RAM

-  200 GB for Volume (e.g. non ephemeral) storage

Allocation of more resources for UniPD users must be approved by the
Cloud UniPD "governance". Mail your request to
cloud-unipd-gov@lists.pd.infn.it if you want more resources to be
allocated to your project.

.. NOTE::

    Public (i.e. not private) projects are projects where other users
    can apply for membership. They are supposed to be used for
    experiments or other research groups.

    **Personal private projects are discouraged** and are created only
    for convincing reasons.


.. NOTE::

    The person who asks for the creation of a new project is
    automatically defined as the manager of this project, i.e. he/she
    will have to manage the membership requests for this project. So the
    request to create a new project should be done by the relevant
    experiment/group leader.


When you have filled the form, please read the AUP that you need to
accept (by clicking the **Accept AUP** button).

Finally click on the **Register** button and you are done.


.. image:: ./images/RegistrationDone.png
   :align: center



Your request will be managed by the Cloud adminstrator and by the
manager(s) of the project(s) for which you applied membership. You will
get an e-mail when your request is approved (and therefore you can start
using the CloudVeneto) or if for some reason your request is refused.



Apply for other projects
------------------------
.. _ApplyForOtherProjects:


After you have been given an account on the CloudVeneto, at any time you
can ask the creation of a new project or the membership to an already
existing project.

Both operations are performed by accessing the 
**Identity** |rarr| **Projects** tab of
the OpenStack dashboard and clicking on **Subscribe to project** as depicted
on the following image:


.. image:: ./images/ProjectRequest-new.png
   :align: center


Fulfill your request selecting the relevant choice under the **Project
action** dropdown list.

Manage project membership requests (only for project managers)
--------------------------------------------------------------
.. _ManageProjectMembershipRequests:

If you are the manager of a project, you will receive membership
requests for this project that you will have to manage (approving or
refusing them).

When a user applies to be member of a project that you manage, you will
receive an e-mail such as this one:

.. image:: ./images/email_subreq.png
   :align: center



To manage such requests, open the OpenStack web dashboard, i.e. go to
https://cloud-areapd.pd.infn.it or https://cloudveneto.ict.unipd.it in a
browser. Log in, and then access **Identity** |rarr| **Subscriptions**. 
An image such as
the following one, with the list of the pending requests, will appear.

.. image:: ./images/Subscriptions.png
   :align: center



To approve a membership request, click on the **Approve** button (in
**Actions**). A window such as the following one will appear:

.. image:: ./images/ProcessSubscription.png
   :align: center


Set the expiration date of the account, and click on the **Ok** button to
approve the request.

If, instead, you want to reject the request, select **Reject** in **Actions**.

.. NOTE::

    It is therefore up to the project manager to set the expiration date
    of the members of his/her group.

    A user belonging to multiple projects can have different expiration
    dates for the different projects he/she belongs to.

Administer project members (only for project managers)
------------------------------------------------------
If you are the manager of a project, you can list the members of your
project and, if needed, change their role.

Open the OpenStack web dashboard, i.e. go to
https://cloudveneto.ict.unipd.it/dashboard in a browser. Log in using
the relevant method and access the **Identity** |rarr| **Project Members** 
panel. The
list of users affiliated to your project will appear:


.. image:: ./images/IdentityProjectMembers.png
   :align: center


From here you can also change the role of a specific user (by clicking
on **Toggle Role**) from 'Project User' to 'Project manager' or viceversa.

.. NOTE::
    If a user is promoted to Project manager, she will then be allowed
    to manage affilitation requests to the project, as described in 
    :ref:`Manage project membership requests (only for project managers)<ManageProjectMembershipRequests>`.

From this window you can also remove a specific user from the project
you manage.

Manage account renewals (only for project managers)
---------------------------------------------------

When the affiliation of a user for a project is expiring, as manager of
that project you will receive an e-mail such as this one:

.. image:: ./images/email_renewreq.png
   :align: center


To manage such requests, open the OpenStack web dashboard,
i.e. go to https://cloud-areapd.pd.infn.it or
https://cloudveneto.ict.unipd.it in a browser. Log in, and then access
**Identity** |rarr| **Subscriptions**. An image such as the following one will appear:

.. image:: ./images/renew_acc.png
   :align: center

Click on the **Renew** button (in **Actions**). A window, such as the one
represented in the following image will appear:

.. image:: ./images/renew_setdate.png
   :align: center


Set the new expiration date and then click the **OK** button.

Expired users
-------------
Please note the resources (instances and volumes) owned by expired users 
(i.e. people who
don't have anymore an account on CloudVeneto) will be removed.

Please also note that, while the ownership of a 
volume can be transferred from a user to another one 
(see :ref:`Transferring the ownership of a volume to another user<TransferVolume>`), this can't be technically possible
for virtual machines.

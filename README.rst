========================
Team and repository tags
========================

.. image:: https://governance.openstack.org/badges/i18n-specs.svg
    :target: https://governance.openstack.org/reference/tags/index.html

.. Change things from this point on

=============================
OpenStack I18n Specifications
=============================

This git repository is used to keep track of design specifications
with reviews and changes to the OpenStack I18n program.
Reviews of the specs are done in gerrit, using a similar workflow to
how we review and merge changes to openstack/i18n repository.

Expected Work Flow
==================

1. Create a blueprint in https://blueprints.launchpad.net/openstack-i18n
   with a task affecting the ``i18n-specs`` project.
2. Propose a change to i18n-specs repository.
   You can find an example spec in `/template.rst`.
   Fill it and create a .rst file in `/specs/` directory with the details
   of the new blueprint
   (ensure "Implements: blueprint [blueprint name]" is in the commit message).
3. Review happens on proposal by i18n-core members and others.
4. When ready for final approval, bring forward the proposed item to
   the i18n IRC meeting or mailing list: openstack-i18n@lists.openstack.org.

Once a specification is approved...

1. Leave a comment to the git address of the specification
   on the blueprint.
2. Indicate "Implements: blueprint [blueprint name]" on the commit messages
   for related implementations.


For i18n, blueprints are required for larger, cross- and coordinated projects but
not for small translation fixes. It's a judgement call for whether you need a
spec, so feel free to ask in the
#openstack-i18n IRC channel or on the openstack-i18n mailing list.

Prior to the Ocata development cycle, this repository was not used for spec
reviews. Reviews prior to Ocata were completed mainly through `Launchpad
blueprints <http://blueprints.launchpad.net/openstack-i18n>`_.

Please note, Launchpad blueprints are still used for tracking the
current status of blueprints. For more information, see
https://wiki.openstack.org/wiki/Blueprints.

For more information about working with gerrit, see
http://docs.openstack.org/infra/manual/developers.html#development-workflow.

To validate that the specification is syntactically correct (i.e. get more
confidence in the Jenkins result), please execute the following command::

  $ tox

After running ``tox``, the documentation will be available for viewing in HTML
format in the ``doc/build/`` directory. Please do not check in the generated
HTML files as a part of your commit.

The files are published at http://specs.openstack.org/openstack/i18n-specs.

The git repository is located at
http://git.openstack.org/cgit/openstack/i18n-specs/.

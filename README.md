To do
=====

* Churn through 400 old emails.
* Can we make the filter pop-up turn to "advanced" and dim itself when the user does something so crazy we can't a make useful characterization of it? Is there even such a thing?
    function:foo regexp:bar
* Should we change from mixterms to maxterms to be like Google?
* Should I go to MozFest?


Done
====

2013-08-15
----------

* More reviewing of omniglot patch
* Captain Shove meeting
* More designing of Shiva's shape

2013-08-14
----------

* Began reviewing omniglot: VCS integration for DXR.
* Began design of Shiva The Deployer's shape. Determined that [Shiva itself cannot be the top-level entrypoint into deployment](https://github.com/erikrose/shiva/issues/1#issuecomment-22663747).
* Noticed http://collabedit.com/jbt8n, which is an Etherpad-alike with syntax highlighting.

2013-08-13
----------

* Got Schalk started on the new DXR UI. First, we're going to rip out the useless splash page. We'll have to figure out where to put the browsing interface. Will it be hard to do what the wireframes say initially? Then we'll implement basic search. We'll create a `ui` branch and deploy all this on stage and see how people like it.
* Research talk on [dynamic analysis of JS](https://air.mozilla.org/test-and-cure-your-javascript-blues-with-jalangi/)
* Started Shiva The Deployer as a separate project. Added issues. Inducted rhelmer into my insanity.
* [DXR will no longer deploy broken builds](https://bugzilla.mozilla.org/show_bug.cgi?id=886463).
* Wrote a [justification of Captain Shove](https://wiki.mozilla.org/Websites/Captain_Shove#Justification), because I was having doubts myself.

2013-08-12
----------

* solarce persuaded me [https://github.com/mozilla/captain/issues/4#issuecomment-22528497](back to my original) position on Shove.
* Participated in the Compensation discussion.
* [Revised dxr.sh patch](https://bugzilla.mozilla.org/show_bug.cgi?id=886463) to exit with status 2 so the TBPL tree turns red instead of orange.
* Discussed Captain Shove's need for a custom Shove with solarce.
* Chewed through another 100 old emails. 169 to go!
* Asked jcranmer to ping catlee or rails to review the dxr.sh patch that should keep DXR's index from getting corrupted on failed builds.
* Made [https://bugzilla.mozilla.org/show_bug.cgi?id=705745](an old bug) go away.

2013-08-09
----------

* Polished up rev. 2 wireframes and [https://wiki.mozilla.org/DXR_UI_Refresh](published them) for feedback.
* Solicited feedback from the usual suspects on IRC and from dev-static-analysis@.
* Tried to find a "panacea" advanced search which doesn't necessitate fancy parsing.
* Rendered feedback on willkg for Ricky.

2013-08-08
----------

* Solved the last few problems in the rev. 2 DXR UI mockups.
* Churned through 100 more old emails.
* Talked with Lars about the state of RabbitMQ in Socorro. Discussed the future of reprocessing.

2013-08-07
----------

* Theorized about a cause for some [`derived` searches not working](https://bugzilla.mozilla.org/show_bug.cgi?id=885977).
* Churned through 100 old emails.
* Gave rhelmer a crash course on my in-vitro deployment IoC framework.
* Considered SaltStack for part of Captain Shove.
* Registered for Summit
* [My Fifth Elephant keynote](https://hasgeek.tv/fifthelephant/2013-2/631-what-happens-when-firefox-crashes) is up!
* Made sure today's DXR instance deployment worked properly.
* Posted a patch to the shell script around dxr-build so failed builds don't [end up in a deploy](https://bugzilla.mozilla.org/show_bug.cgi?id=886463).


2013-08-06
----------

* Reviewed [MXR malware-hosting](https://bugzilla.mozilla.org/show_bug.cgi?id=628033>) fix. Fubar is merging and deploying it.
* Ran the WebDev Extravaganza.
    * peep makes your downloads trustworthy,
        * so we can use PyPI (and its new CDN, which makes it reasonably reliable).
        * You don't have to trust authors.
        * So it's like a "pip freeze" with teeth.
* Chased [spurious DXR build publishing](https://bugzilla.mozilla.org/show_bug.cgi?id=886463) that happened despite a build failure.
* Invited non-employees to WebDev Extravaganza.

2013-08-05
----------

* Make GH status repo.
* Sent out invite to WebDev Extravaganza. Put pyelasticsearch 0.6 release, django-nose co-maintainer solicitation, and discussion of the future of crypto-verified repeatable Python deployments on the agenda.
* First round of simplified DXR UI refresh wireframes

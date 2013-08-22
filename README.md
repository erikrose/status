To do
=====

* Churn through 400 old emails.
* Can we make the filter pop-up turn to "advanced" and dim itself when the user does something so crazy we can't a make useful characterization of it? Is there even such a thing?
    function:foo regexp:bar
* Should we change from minterms to maxterms to be like Google?
* Should I go to MozFest?
* If Lars hasn't finished the Rabbit stuff by the last day of August, make sure he's handed it off to me.
* [Revise DXR's plugin API to require less boilerplate and fewer singletons](https://bugzilla.mozilla.org/show_bug.cgi?id=883363).
* Consider esprima as a JS parser.
* Lead How to Avoid Burnout BoF at Summit. potch: "Don't let someone else win the Martyrdom Olympics". Laura is interested. Also, First International Symposium On Bikeshedding About Shit No One Is Ever Going To Fix. :-)
* _all index: https://github.com/rhec/pyelasticsearch/issues/127
* Distribution.from_location, .version, .project_name. content_type = pip.mimetypes.guess_type(path)[0]
  Or maybe I can avoid untarring each archive again and just reparse the version and package name out of reqs.txt. Every downloaded filename has to be package_name + version + some archive extension.
  Then comment on https://bugzilla.mozilla.org/show_bug.cgi?id=894493.
* Review https://github.com/mozilla/shove/pull/4.
* Write a failing test against some kind of playground environment to expose Thrift failures. Once that's failing, we can do experiments to figure out what's wrong. We can probably get Thrift installed on Mango, another HBase cluster. Whose fault is it? Zeus? Python? Java?


Done
====

2013-08-21
----------

* Confirmed my fix made peep work on Windows.
* Triaged pyelasticsearch PRs. Merged a couple of small ones.
* The hash output in peep now includes the actual version numbers of packages,
  so you can just paste it straight into your requirements.txt.
* Helped rhelmer switch Socorro's deployment to peep.
* Don't indent the hash output so you don't have to dedent when pasting into reqs.txt.

2013-08-20
----------

* https://pypi.python.org/pypi/configobj/ is great! It's the ConfigParser rewrite I was going to do. Now I don't have to!
* Reviewed https://github.com/mozilla/shove/pull/3/files.
* [Switched to a console_scripts entrypoint in peep](https://github.com/erikrose/peep/issues/8), which should make it Windows-compatible.
* With Adrian, designed a new Socorro ES schema for raw+processed dumps.

2013-08-19
----------

* Chased a pyelasticsearch bug Adrian ran into where he couldn't search all indices simultaneously.
* Meetingsmeetingsmeetings

2013-08-18
----------

* Started coding up Shiva's deployment framework and the command-line tool.

2013-08-16
----------

* Reorganized Shiva code. Got commandline tool stubbed out. Eggified.

2013-08-15
----------

* 1:1
* More reviewing of omniglot patch
* Captain Shove meeting
* Figured out [Shiva's shape](https://github.com/erikrose/shiva/issues/1#issuecomment-22725248).

Week Summary
------------

* [DXR no longer has a day of downtime when its index fails to build](https://bugzilla.mozilla.org/show_bug.cgi?id=886463).
* Started Shiva The Deployer to factor our common deployment script functionality and make deployment more robust.
* Finished [https://wiki.mozilla.org/DXR_UI_Refresh](DXR wireframes).
* Got Schalk started on the new DXR UI. First, we're going to rip out the useless splash page. We'll have to figure out where to put the browsing interface. Will it be hard to do what the wireframes say initially? Then we'll implement basic search. We'll create a `ui` branch and deploy all this on stage and see how people like it.


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

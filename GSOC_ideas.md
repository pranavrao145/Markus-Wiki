================================================================================
Google Summer of Code Ideas
================================================================================


Here is the summary of all the ideas we have for GSoC

.. contents::

Performance analysis 
================================================================================

As we begin to use MarkUs is classes larger than 500 students, we need to get a better picture of the performance limitations, and what we can do to mitigate them. If a large number of students try to submit their assignments using MarkUs in a short time window, where are the performance bottlenecks? Rails? The database? Subversion?

This project would involve setting up a test environment, profiling, and stress testing MarkUs. An applicant should have enough Linux knowledge to be able to set up concurrent tests and measure performance, and enough database knowledge to be able to do some profiling. Basic Ruby and Rails knowledge, web application knowledge would be a strong asset. (We realize this is a lot to ask, but for the right student, this could be a really rewarding project.)

Integrating Git, bzr and hg to Markus
================================================================================

Markus can be configured either to allow students to submit code through a
web interface, or to provide students an svn repository. As DCVS
becomes more and more popular, students often use svn2X tools in order to
use DCVS, hosting the code in plateforms like github, launchpad or
bitbucket. The idea would be to create an interface for Markus to retrieve
automatically the code to be graded (student providing a url).

Requirements for this project are good familiarity with at least one DCVS, and preferably some experience with Ruby to explore the library bindings.

Web based PDF annotations
================================================================================

Markus has a web-based PDF annotations module that uses [ImageMagick](http://www.imagemagick.org/script/index.php) to convert a pdf file into an image, in order to be able to annotate it. There are several limitations to this approach: the pdf document is limited to 30pages, substantial processing time is required to perform the conversion, documents cannot easily be viewed in different sizes. This project is of an exploratory nature, to find a better solution to pdf annotations.


Mapping Graders to Groups
================================================================================

The facility in MarkUs that maps Graders to the groups that they are responsible for marking currently provides only very simple mapping functions. Professors can either assign graders randomly to groups, or can upload a specific mapping. We have had requests to implement more sophisticated mapping ability.  For example:

- Map graders favoring students previously graded by these graders
- Map graders favoring students NOT graded by these graders
- Map graders to all students of one section
- Map graders randomly to all students of a section

This project will require Ruby and Rails skills. It will involve some interesting UI work, but should be a fairly straightforward project. A student who chooses this project will also end up working on several other small projects.

Integrated documentation system
================================================================================

As the user base for MarkUs grows, the need for better documentation becomes clear. It will be an interesting software design problem to create an integrated documentation system that tracks versions and configurations.

This project requires some Ruby/Rails knowledge and a desire to create simple, elegant software.

A VM harness for the automated test framework
================================================================================

We have been working towards an automated test framework that
            allows students to submit their work and receive immediate feedback.
            To run student submitted code on a server, we need to think
            carefully about how to do this securely. Running the tests inside a
            locked down VM seems to be the most promising solution. 

This project requires Linux and VM knowledge, preferably with
            some system administration skills.



Integrated doc/odt support
================================================================================

Convert doc or odt into images, or plain text in order to be able to annotate
them.


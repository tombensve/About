# About - General info about all my repos

My GitHub repos are partly for need, but mostly a place were I'm having fun!

It is so far only Java, Groovy and some JS here. I have decided to use Groovy
as much as possible, because it is a superb language and completely compatible 
with Java! You can write better code in Groovy than with Java, and Groovy have 
always had features that Java didn't get until 1.8, and Groovy still does it 
better! The people behind Groovy know what they are doing! 

Some project produce binary jar files that I have decided to make available
on my web server after bintray shut down: `https://download.natusoft.se/maven`.
This URL can be specified as a repo in maven pom.xml:

    <repositories>
        <repository>
            <id>tombensve-repo</id>
            <name>tombensve-artifact-repository</name>
            <url>https://download.natusoft.se/maven</url>
        </repository>
    </repositories>

    <pluginRepositories>
        <pluginRepository>
            <id>tombensve-plugin-repo</id>
            <name>tombensve-plugin-repository</name>
            <url>https://download.natusoft.se/maven</url>
        </pluginRepository>
    </pluginRepositories> 

## No more Windows in my future!

I've been a long time Linux user. I used to only update kernel once a year so that I could do an
`uptime` command and get `365` back :-). It never crashed and never needed restart unless kernel 
update was required. But then I went over to Mac and still run some Linux in Parallels.

I have Java and Groovy code in my GitHub repos. Probably more Groovy than Java. The JVM platform
should be _platform independent_ and between Mac and Linux it pretty much is! 

When it comes to windows compared to unixes however there have been "platform" issues, where
things behave differently. I made a Swing GUI for a Markdown editor I made as part of my
MarkdownDoc repo. The first time I ever ran that editor on Windows there were clear differences
in behavior. 

My current Mac is and M1 Max Pro with
10 cores and 64 GB memory. A very competent machine! It is however using an ARM64 and not AMD64
processor architecture. I only have an AMD64 version of a windows 10 and ARM64 version of 
Windows 11 that can be run in Parallels does not seem to be available. I have spent many hours 
on trying to solve getting an ARM64 image of Windows 11, and then buy a windows license for it,
but I have failed to find how to get an ARM image of windows 11. It might be restricted to
Microsofts Surface tablets.

Until Windows becomes a Linux distro there will be compatibility problems!

I have now decided to not waste any more time on this, and can no longer test / verify anything
on windows! If it works, then fine. If it doesn't then there is not much I can do!   

## Why not maven central ? 

Well, I did that once and that was an absolutely
horrible process to go through! I sent a mail to maven users list saying
that releasing to maven central must be an easier process. I got only one
answer, and that was from JFrog asking if I had seen bintray. I had not,
and took a look. I became a user immediately. JFrog understood how easy
this process really should be!! I have no idea why they shut down the
bintray service, it was one of the best I've ever used! 

Submitting to maven central have (from googling) become a little bit
easier, but after reading up on the whole procedure I conclude that 
it is still a far too complicated process. My GitHub code is mostly 
for fun and it need to continue to be that. I don't want to feel a 
knot in my stomach when I need to release a new version. So thereby 
I publish binaries on my web that maven can use as a repo. A new free 
repo with bintrays simplicity is really needed. I think that maven is 
an absolutely brilliant piece of software! But Sonatype need to 
rethink their handling of maven central.

It is also possible to checkout my repo and build it with `mvn install`. After that there will be binareis
in your ~/.m2/ folder. 


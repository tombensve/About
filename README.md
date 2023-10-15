# Tommy Bengt Svensson

I'm a software developer that wrote my first code on a [Sinclair ZX-80 machine](https://en.wikipedia.org/wiki/ZX80)
when I was 12. When I was 13 I got the ZX81, which also could display information on the screen at the same time as
processing! :-). At 14 my family moved from Stockholm, Sweden to Seattle, USA. There I got a TRS-80 Color Computer made
by Tandy. It had a total of 8 colors! It also had a Motorola 6809 processor and could thereby run the OS9 fully
multitasking operating system, very much inspired by unix. Its C compiler even used the unix names for system calls
so that much unix code could be compiled on it. 

I  moved back to Sweden when I was 21. Eventually starting my career at Ericsson, where I had no problems
comprehending the SUN Unix machines since it felt very much like OS9. 

I wrote C code at the beginning, but became a consultant later and happend to be in a project using Java 1.0.
Be glad if you missd that! But Java has gotten better and better over time. I am however not in agreement with Oracles
descicion to skip backwards compatibility from 12 and upp! I think that was stupid! So far no place I've been
as a consultant have gone past Java 11! That says something IMHO. Java 6 was seen as a very good release. That 
is because it took 5 or 6 years until Java 7. That provided stability! 

## My GitHub repos

Are partly for need, but mostly a place were I'm having fun and stimulating my brain.

It is so far only Java, Groovy and some JS here. I have decided to use Groovy
as much as possible, because it is a superb language and completely compatible 
with Java! You can write better code in Groovy than with Java, and Groovy have 
always had features that Java didn't get until 1.8, and Groovy still does it 
better! The people behind Groovy know what they are doing! 

## Binaries

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




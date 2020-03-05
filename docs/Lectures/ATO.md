<div id="column">

<div id="content">

<div id="pageContent">

## ATO Manual

The ATO is the approved method used to task and disseminate to components, subordinate units, and command and control agencies projected sorties/capabilities/forces to targets and specific missions.  The ATO describes essential task information for the COMAO, such as objectives, participating forces, target, time frame, Rules of Engagement, deconfliction parameters, etc., as well as general instructions. The ATO gives a summary of active flights in the upcoming COMAO event for a 24 hour period. This document describes how to read ("frag") the contents of an ATO.

### Format

Each line of a tasking contains a _set_ of information. The line starts with the name of the current set and is followed by a number of _fields_. Each field contents are separated by a forward slash, /. Field values are plain-text, human-readable information, or a - to signify an empty value. The line is terminated by two consecutive forward slashes, //.

**Example:**

<pre>AMSNDAT/AI2362/AI/CAS/-/28/-/1911/DEPLOC:URSS/ARRLOC:URSS//</pre>

**Interpretation:** _Air mission data for mission number AI2362 performing an Air Interdiction (AI) primary mission followed by a Close Air Support (CAS) secondary mission, operating without a package, with pilot ID 28 as a mission commander, no alert-state condition, takeoff time at 1911 ZULU, departing from and recovering at Sochi-Adler international airport (ICAO code URSS)._

### Sets

A tasking order consists of several of the following sets:

*   OPER: Operation
*   MSGID: Message identification
*   PERIOD: ATO from-to time
*   TASKUNIT: Tasked unit
*   AMSNDAT: Air Mission Data
*   GTGLOC: Ground Target Location
*   PKGCMD: Package Commander
*   ARINFO: Air to Air Refueling
*   CONTROLA: Controlling agency
*   FACINFO: Forward air controller
*   NARR: Explain preceeding  reference text

Not all sets are mandatory. At minimum TASKUNIT, AMSNDAT and MSNACFT are required for a valid tasking.

### Fields

Each set contains a number of _fields_ of information:

*   OPER/operation name/plan originator and number//
       
    <pre>OPER/VIRTUAL TLP/COURSE 19-1//</pre>

*   MSGID/ATO/originator/message serial number/month/qualifier/qualifier serial number//

    <pre>MSGID/ATO/VIRTUALTLPSTAFF/-/NOV/TLPv CONFIDENTIAL/-//</pre>

*   PERIOD/FROM: time from/TO: time to//

    <pre>PERIOD/FROM 180000ZNOV18/TO182359ZNOV18//</pre> 

*   TASKUNIT/tasked unit designator/ICAO location/comments//
    
    <pre>TASKUNIT/VIRTUAL TLP OPS/ICAO: LEAB/-//</pre>

*   AMSNDAT/mission number/package identification/aircraft call sign/number and type aircraft/mission type/alert status/primary configuration code/secondary configuration code/iff-sif code and mode//

    <pre>AMSNDAT/40RJ1626/PACKAGE “HOTCHILI”/PHANTOM/COBRA/DEVIL/2F16/2F16/2F16/AI/-/4GB12/-/-//</pre>
     
*   GTGLOC/Designator/Time on target/Not earlier than/Not later than/Target name/Target ID/Target type/DMPI description/Desired Mean Point of Impact/DMPI elevation/Target priority//

    <pre>GTGTLOC/P/-/NET:060900ZMAR/NLT:060905Z/RED BLUFF AFLD /ID:0992-00101DD001/-/DISPERSAL AREAS/DMPID:400948.0N1221406.0W/-/-//</pre>
    
    <pre>GTGTLOC/SEE TARGET FOLDER QW-300/TOT0800Z0830Z/DPI 1-13/PRIO GRADE 1/CDE1LOW/PGM/INSTANT//</pre>
    
*   PKGCMD
    1.  Package
    2.  Tasked unit
    3.  Msn number
    4.  CALLSIGN
    
*   REFUEL
    1.  CALLSIGN
    2.  Position
    3.  Altitude
    4.  Frequency
    5.  TACAN
    
*   CONTROLA
    1.  Type
    2.  CALLSIGN
    3.  Report in point
    4.  Primary Frequency
    5.  Secondary Frequency
    
*   FACINFO/call sign/primary (frequency) or (frequency designator)/secondary (frequency) or (frequency designator)/report-in point/support unit identity/control comments//
*   NARR/free text to explain preceding reference set//
   

</div>

</div>

</div>

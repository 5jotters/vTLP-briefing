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
*   TASKUNIT: Tasked unit
*   AMSNDAT: Air Mission Data
*   MSNACFT: Mission Aircraft
*   AMSNLOC: Air Mission Location
*   GTGLOC: Ground Target Location
*   PKGCMD: Package Commander
*   ARINFO: Air to Air Refueling
*   CONTROLA: Controlling agency
*   TAC: Terminal Attack Controller
*   NARR: Explain preceeding  reference text

Not all sets are mandatory. At minimum TASKUNIT, AMSNDAT and MSNACFT are required for a valid tasking.

### Fields

Each set contains a number of _fields_ of information:
*   OPER
    1. Operation name
    2. Plan originator and number
    
    <pre> OPER/VIRTUAL TLP/COURSE 19-1//</pre>

*   TASKUNIT
    1.  Tasked unit designator
    2.  ICAO location
    
    <pre> TASKUNIT/VIRTUAL TLP OPS/ICAO: LEAB//</pre>

*   AMSNDAT
    1.  Msn Number
    2.  Primary Mission
    3.  Secondary Mission
    4.  Package
    5.  Commander ID
    6.  Alert State
    7.  Takeoff Time (in-game time)
    8.  Departure Airfield/Location
    9.  Recovery Airfield/Location
*   MSNACFT
    1.  Number of Aircraft in Flight
    2.  Type of Aircraft
    3.  Callsign and Flight Number
    4.  Primary Config
    5.  Secondary Config
    6.  Primary Frequency
    7.  Secondary Frequency//
*   AMSNLOC
    1.  Time From
    2.  Time to
    3.  Position
    4.  Altitude
*   GTGLOC
    1.  Designator
    2.  Time on target
    3.  Not earlier than
    4.  Not later than
    5.  Target name
    6.  Target ID
    7.  Target type
    8.  DMPI description
    9.  Desired Mean Point of Impact
    10.  DMPI elevation
    11.  Target priority
*   PKGCMD
    1.  Package
    2.  Tasked unit
    3.  Msn number
    4.  CALLSIGN
*   ARINFO
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
*   TAC
    1.  Type
    2.  CALLSIGN
    3.  Position
    4.  Primary Frequency
    5.  Secondary Frequency
*   AMPN
    1.  Amplification

</div>

</div>

</div>

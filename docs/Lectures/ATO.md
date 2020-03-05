## How to read the ATO

The ATO is the approved method used to task and disseminate to components, subordinate units, and command and control agencies projected sorties/capabilities/forces to targets and specific missions.  The ATO describes essential task information for the COMAO, such as objectives, participating forces, target, time frame, Rules of Engagement, deconfliction parameters, etc., as well as general instructions. The ATO gives a summary of active flights in the upcoming COMAO event for a 24 hour period. This document describes how to read ("frag") the contents of an ATO.

### Format

Each line of a tasking contains a _set_ of information. The line starts with the name of the current set and is followed by a number of _fields_. Each field contents are separated by a forward slash, /. Field values are either information in plain-text, or a - to signify an empty value. The line is terminated by two consecutive forward slashes, //.

**Example:**

<pre>AMSNDAT/40RJ1626/PACKAGE “HOTCHILI”/PHANTOM/COBRA/2F16/2F16/AI/-/0630Z/DEPLOC:LEAB/ARRLOC:LEAB/4G12/-/-//</pre>

**Interpretation:** _Air mission data for mission number 40RJ1626, PHANTOM and COBRA, two 2-ship F16 flights, operating withing package HOTCHILI, performing an Air Interdiction (AI) mission, no alert-state condition, take-off at 06:30 zulu, departing from and recovering at LEAB, ordnance 4 GBU 12 without secondary configuration, no IFF specified.

### Sets

A tasking order consists of several of the following sets:

*   OPER: Operation
*   MSGID: Message identification
*   PERIOD: ATO from-to time
*   TASKUNIT: Tasked unit
*   AMSNDAT: Air Mission Data
*   GTGLOC: Ground Target Location
*   REFUEL: Air to Air Refueling
*   CONTROLA: Controlling agency
*   NARR: Explain preceeding  reference text

Not all sets are mandatory. At minimum TASKUNIT and AMSNDAT are required for a valid tasking.

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

*   AMSNDAT/mission number/package identification/aircraft call sign/number and type aircraft/mission type/alert status/take off time/Departure Location/Arrival Location/primary configuration code/secondary configuration code/iff-sif code and mode//

    <pre>AMSNDAT/40RJ1626/PACKAGE “HOTCHILI”/PHANTOM/COBRA/2F16/2F16/AI/12H/0630Z/DEPLOC:LEAB/ARRLOC:LEAB/4G12/-/-//</pre>

*   GTGLOC/Designator/Time on target/Not earlier than/Not later than/Target name/Target ID/Target type/DMPI description/Desired Mean Point of Impact/DMPI elevation/Target priority//

    <pre>GTGTLOC/P/-/NET:060900ZMAR/NLT:060905Z/RED BLUFF /ID:0992-001/-/DISPERSAL AREAS/DMPID:400948.0N1221406.0W/-/-//</pre>
    
*   GTGLOC/TGT folder/Time on target/Target name/Target ID/Target priority/accuracy of coordinates/ammunition type/fuze//
    
    <pre>GTGTLOC/SEE TGT FOLDER QW-300/-/NET:0800Z/NLT:0830Z/-/DPI 1-13/PRIO GRADE 1/CDE1LOW/PGM/INSTANT//</pre>

*   C2TASK/mission number/package identification/aircraft call sign/number and type aircraft/aircraft capability//

    <pre>C2TASK/-/PACKAGE “ALHAMBRA”/MAGIC/1E3/C2//</pre>

*   REFUEL/callsign/tanker mission number/aar control point/altitude/aar control time/frequency/tacan// 
    
    <pre>REFUEL/CAMEL/C3/FL200/0800Z1030Z/269.0/2Y//</pre>
    
*   CONTROLA/type of control/call sign/primary frequency/secondary frequency/report-in point/comments//

    <pre>CONTROLA/BOT/COBRA/235.6/-/E5/-//</pre>
     
*   NARR/free text to explain preceding reference set//

    <pre>NARR/SEAD COMMANDER: PHANTOM//</pre>

## ADDITIONAL INFORMATION 
The ATO can give other information relative to SPINS, ROE, ACO, etc. This section can be as long as needed.

#### C2 BATTLE MANAGEMENT PLAN/
<pre> 
  2. TAC C2 REMARKS:
       A. A NOTIONAL IFF MODE 1 AND MODE 4 WILL BE USED BY BLUE FORCES//
       B. “ALHAMBRA” PACKAGE USE MODE 1=11 AND A CORRECT MODE 4//
       C. AUTHORITY TO ENGAGE IS DELEGATED TO WEAPON PLATFORMS//
       D. LINK-16 NTR WILL BE THE MISSION HOST//
       E. AUTHENTICATION WILL BE PRIMARILY BASED ON VIRTUAL TLP AMSL 1800//
       F. USE BULLSEYE CALLSIGN “BULLSEYE”//
       G. OUTLAW DEFINED ANY CONTACT GENERATED BEYOND THE FLOT//
       H. LOW DEFINED AS BELOW 5000’ AMSL, SLOW DEFINED AS LESS THAN 300KGS//
</pre>

#### RULES OF ENGAGEMENT (ROE)/
<pre> 
  4. ROE REMARKS:, THE FOLLOWING ROES ARE APPLICABLE:
       A. 007, 008, 010//
       B. AG: 101,102,103,104//
       C. SEAD: 200, 201, 202//
       D. ECM: 130//
       E. SBAD: WEAPONS FREE INSIDE BLUE TERRITORY//
</pre>

#### COMPOSITE AIR OPERATIONS (COMAO) PLAN/
<pre> 
PKGINFO “ALHAMBRA”/-/-//
/
UNIT	       	MISSION	      	 C/S	       Nº TYPE	       	REMARKS

ALBACETE	40RJ1901	SPARTAN	       2 x EF2k		SWEEP/ESCORT
	       	40RJ1902	LOBO	       2 x F16		SWEEP/ESCORT
	       	40RJ1903	COBRA	       2 x F16		SWEEP/ESCORT
	       	40RJ1904	PHANTOM	       2 x F16		SEAD
	       	40RJ1905	FALCON	       2 x F16		SEAD
	       	40RJ1906	ROCKET	       2 x F16		PP CAS
	       	40RJ1907	DEVIL	       2 x F16		PP CAS
	       	40RJ1908	BRONCO	       2 x F16		PP CAS
	       			
				
	       	40RJ1911	CHALIS	       1 x E-3		AWACS
	       	40RJ1912	CAMEL	       1 x KC-10	AAR
	       	40RJ1913	CANTEEN	       1 x KC-135	AAR
	       	40RJ1914	CHARGER	       1 x KC-10	AAR
/
PACKAGE TASK:
       A.	PP CAS: SCUD MISSILES SITES//
       B.	SEAD: PROTECT PACKAGE “ALHAMBRA”//
       C.	OCA: PROTECT PACKAGE “ALHAMBRA”//
/
</pre>


#### ADDITIONAL SPECIAL INSTRUCTIONS/
<pre> 
  3. RISK LEVEL:
      A. VIRTUAL TLP COALITION USE RISK LEVEL MEDIUM//
</pre>


#### AIRSPACE CONTROL INFORMATION/
<pre> 
  1. AIRSPACE CONTROL INFORMATION:
     A. DEPARTURE AND RECOVERY ACCORDING TO LOCAL PROCEDURES//
     B. HOLDING AREA ESTABLISH FROM FL100 TO FL380 FOR PACKAGE “ALHAMBRA”
         i.	CHALIS WILL MAINTAIN ASSIGNED ORBIT IAW COORDINATION BRIEF AT FL300//
         ii.	AIRCRAFT DEPARTING ALBACETE WILL NOT CLIMB ABOVE FL150 BEFORE WPT 2 IF THEY ARE GOING TO REFUEL WITH THE NORTHERN TANKER//
         iii.	AIRCRAFT DEPARTING ALBACETE WILL CLIMB TO FL210 MAXIMUM IF THEY ARE GOING TO REFUEL WITH THE SOUTHERN TANKER//
     C. DESIGNATED SWEEP/ESCORT/SEAD/AI FORCES OF PACKAGE “ALHAMBRA” USE SAME ROUTE FOR THE PUSH AT THE ASSIGNED ALTITUDE//
     D. DESIGNATED SWEEP/ESCORT/SEAD/AI FORCES WILL DEPARTURE VMC//
</pre>
#### RMKS/
<pre> 
  5. TLP REMARKS:
     A. ALL TIMES GIVEN ARE MANDATORY//
  /
  6. GENERAL REMARKS:
     A. NO TAKE OFFS BEFORE 0630Z//
     B. IT IS NOT EXIST RECOVERY TIMES. FORMATION SHOULD ADJUST 2NM TRAIL BETWEEN THEM AS MINIMUM.
     C. ALL CREWS ARE TO CARRY MISSION MAPS AND ALL DOCUMENTATION PROVIDED BY MC//
</pre>

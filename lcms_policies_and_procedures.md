Title:  GNPN / ChEM-H shared LC-MS policies and procedures  
Author: Curt Fischer  
Date:   July 18th, 2016    

# GNPN / ChEM-H shared LC-MS policies and procedures  

This document is the current (March 2016) home of the policies and procedures relating to the Agilent 6545 q-TOF mass spectrometer that is shared by ChEM-H and the Stanford Genome Technology Center.

## General rules and guidelines


1. Only trained users can use the instrument.

2. Users must complete the 6545 Run Log when they start their run.

## Samples

1. _All_ samples, even pure standards or blanks, should be filtered.  The small particle sizes of the UPLC-grade columns we routinely use makes them even more prone to clogging than traditional HPLC columns.  

2. I recommend the use of 96-well plates for running samples.  For more than 12-18 samples, the use of 96-well plates is more economical.  There is also an educational component to this recommendation.  Sampling handling procedures, not only in industry but also in academia, increasingly rely on 96-well plates.  

3. I may be able to provide filter plates (96-well format) on request.  Users should plan to provide their own "receiver" plates to hold filtered samples.  (Be sure your plates are compatible with your samples -- polystyrene is not compatible with high concentrations of most organic solvents, for example.).  The supply of autosampler- and solvent-compatible plate covers is limited, as they are made of costly silicone-based materials.  Do not abscond with them.



## Training

Training consists (i) consultation with Curt regarding the purpose and intention of your experiment, with an eye toward methods optimizations that may be appropriate, followed by (ii) an in-person walkthrough of the instrument, ideally during a new user's first run.  

The goal of consulting with me is to make sure we discuss possibilities for chromatographic (and if necessarily, mass spectrometric) methods optimization.  The 1290 LC stack on the instrument provides a UPLC-grade chromatography capabilities.  (This is referred to by some vendors as "UHPLC".)  UPLC can freqently accelerate analysis times by two- to tenfold compared to the traditional HPLC workflows that many users may be accustomed to.  To maximize the value of your time on the instrument, and to make as much time available to the entire user community as possible, it is important to use methods that serve your purposes without being overly long.  Faster analysis times enable you to design experiments with more replicates and/or time points, resulting in better science.  If/when a I implement a queueing system that prioritizes requests based on the instrument time requested, having faster methods will help you get into into the queue faster.

When a single PI’s lab begins to have more than one user of the instrument, I may designate “deputy” trainers from that lab that can train new users on how to run the instrument.  Here is a rough list of current deputy trainers:

* Sattely lab - Ricardo de la Pena and Russ Li
* Sonnenburg lab - Dylan Dodd


## Scheduling

Time allocation on the shared GNPN / ChEM-H LC-MS is scheduled by Google Calendar.  Right now, from Wednesday at 9 am to Friday at 9 am each week is reserved for GNPN usage, with the remainder of the time available for ChEM-H usage.  

* Google Account of calendar _owner_: `gnpn.chemh.lc.ms@gmail.com`
* Google Account password: `qtof6545`
* The calendar is named `GNPN / ChEM-H LC-MS Schedule`

Right now, the schedule is set by individual users blocking off time on the calendar.  I anticipate that we will likely want to move to a queuing system if possible.  

### Ideas for a queue

A queue is attractive because:

* it allows prioritization of requests based several factors, not just the time of sign-up.
* it eliminates the phenomenon of everyone fighting for the next available slot weeks ahead of time, just in case they need it.  You can be sured of getting the soonest possible, best-available time for your run.

A queue, however, is harder to implement and so it is not implemented yet.

My current plan for a queue would be:

1. Users would request a number of hours for which they would like to access the instrument.  This places you in the queue.  
2. Requests in the queue are immediately prioritized by the date of the request, user affiliation and usage history (ChEM-H vs. GNPN, PI, etc.), and the size of the request (shorter runs get higher priority), and possibly other factors.  An exact formula is TBD.
3. On a weekly basis (e.g. Friday morning), the instrument time for the next week would be released.  The highest priority request would be scheduled first, then the  etc., until no further requests can be accommodated for that week.
4. Users would have some capability to indicate preferred or mandatory scheduling constraints.  For example, users would rarely if ever want to have their run begin at 3 am. Other users may have classes, meetings, and other scheduling constraints.
5. Once time is scheduled your place in the queue is lost (except if you are prevented from actually doing your run because of factors outside your control; e.g. instrument malfunction).
6. At the scheduled time you can do your run(s).

(Feedback on these ideas is appreciated, especially at this early stage of development.)

## Starting a run

Suppose you are a trained user with a scheduled time for your run.  What happens next?  Ideally, these things happen:

1. Check that all waste containers are not full and will not become full during your run.  If they are too full, you should know how to empty them.

2. Check that all LC buffer bottles, including "Buffer A", "Buffer B", **the needle wash buffer and the seal wash buffer**, are full enough to last for the duration of your run.  If they aren't full enough, you should know how to add more.

3. Check that both nitrogen supplies are operational.

3. Check that your desired chromatography columns are installed in the correct location on the instrument.  If they aren't, you should know how to swap out columns.

4. Check that the dual AJS ion source is installed.  If it isn't, let Curt know.  At the end of each run (see below), those who use different ion sources should be re-installing the dual AJS ion source.

5. Change all instrument components from "standby" to "on".

6. Calibrate the instrument.

7. Ensure that the column pressure, instrument state, flow rate, and polarity for your run are correctly set.

8. Make sure your worklist includes a shutdown script so that the instrument returns to Standby when your run is over.

9. Fill out one row verifying your completion of these steps on the 6545 Run Log.

10. Begin your run.


## At the end of a run

1. If you used the MMI ion source, remove it from the instrument and install the dual AJS ion source.

2. If you want to keep your samples, remove them from the autosampler.  Samples that are not removed at the end of your reservation are likely to be discarded and are extremely likely to be moved to a room temperature, non-chilled environment.


CF / cf / July 2016
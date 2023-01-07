---
layout: lesson
root: .  # Is the only page that doesn't follow the pattern /:path/index.html
permalink: index.html  # Is the only page that doesn't follow the pattern /:path/index.html
---

<!-- this is an html comment -->

{% comment %} This is a comment in Liquid {% endcomment %}


# Introduction

The goal of this exercise is to compute the cross section of $Z \to \tau \tau$ 
production. As the tau lepton may decay to e, mu, or hadrons there are in fact 6 different final states to be considered. In this exercise, we will focus on those containing at least one hadronically decaying $\tau$ ($\tau_h$): $e+\tau_h, \mu+\tau_h,$ and $\tau_h+\tau_h$. Please choose one. 

* We will identify sources of standard model processes other than $Z \to \tau \tau$  which may mimic our signal, and define event selection to minimize their contribution to our analysis. 
* The background events will be estimated using both simulation and data-driven approaches. 
* We will then prepare a datacard as an input to the [Higgs Combine Tool](https://cms-analysis.github.io/HiggsAnalysis-CombinedLimit/). This datacard will be used to perform a maximum likelihood fit of the expected signal (taken from simulation) and background yields to extract the best fit value of the $Z \to \tau \tau$  cross section. Each student will perform their work in parallel with the other students, and on the final day, we will collectively combine each person's result into a 15-min presentation summarizing our results.

<!-- Introductory slides can be found [here](https://twiki.cern.ch/twiki/pub/CMS/SWGuideCMSDataAnalysisSchoolLPC2023ZTauTauXsec/LongExerciseZTauTau.pdf). -->

Please join the Mattermost chat for discussion and questions: LongExTauTau Mattermost Channel

*The plots and performance curves seen here are for example purposes only, they do not serve in any official capacity.*


> ## Useful Links
> - CMSDAS Indico agenda: <https://indico.cern.ch/event/1088671/>
> - Tau Short exercises: <https://twiki.cern.ch/CMS/S - WGuideCMSDataAnalysisSchoolLPC2022TauShortExercise>
> - Github repository: <https://github.com/fojensen/nanoAOD-tools/tree/cmsdas2022>
> - DeepTau documentation: <http://cms.cern.ch/iCMS/analysisadmin/cadilines?l - ine=TAU-20-001>
> - DeepTau DPS notes from 2019: <https://cds.cern.ch/record/2694158/>
> - Tau POG: <https://twiki.cern.ch/CMS/Tau>
> - NANOAOD documentation: <https://cms-nanoaod-integration.web.cern.ch/integration/master-102X/mc102X_doc.html>
> - nanoAOD-tools: <https://github.com/cms-nanoAOD/nanoAOD-tools>
> - Tau hypernews: hn-cms-tauid, hn-cms-tau-hlt
> - Tau reconstruction performance in Run 2: <https://arxiv.org/abs/1809.02816>
> - Tau reconstruction performance in Run 1: <https://arxiv.org/abs/1510.07488>
> - Z->tautau at 7 TeV: <https://arxiv.org/abs/1104.1617>
> - Z->tautau at 13 TeV: <https://arxiv.org/abs/1801.03535>
{: .callout}


> ## Prerequisites
>
> For these exercises, you need to bring your laptop registered to the [FNAL network link](http://www.uscms.org/uscms_at_work/computing/getstarted/index.shtml), have a working [LPC](https://twiki.cern.ch/twiki/bin/view/CMS/LPC) account [link](http://www.uscms.org/uscms_at_work/computing/getstarted/getaccount_fermilab.shtml), and have a valid grid certificate [link](http://www.uscms.org/uscms_at_work/computing/getstarted/get_grid_cert.shtml).
{: .prereq}


{% include links.md %}

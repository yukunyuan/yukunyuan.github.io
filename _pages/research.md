---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}


## Decentralized Conflicts Resolution


We study the problem of addressing the conflicts across services in urban cities. We design a decentralized negotiation and conflict resolution framework named DeResolver, which allows services to resolve conflicts by communicating and negotiating with each other to reach a Pareto-optimal agreement autonomously and efficiently. Our design features a two-level semi-supervised learning-based algorithm to predict acceptable proposals and their rankings of each opponent through the negotiation. The evaluation results show that our solution achieves much more balanced results, i.e., only increasing the average waiting time of vehicles, the measurement metric of intelligent traffic light control service, by 6.8% while reducing the weighted sum of air pollutant emission, measured for environment control service, by 12.1%, and the pedestrian waiting time, the measurement metric of pedestrian service, by 33.1%, compared to priority-based solution. [ICCPS 2021, TCPS]


## Electric Taxi Charging Coordination​


Our analysis reveals that most e-taxi drivers charge their vehicles only when their batteries are low, and more than half of taxi drivers charge their batteries to full on each charge. To satisfy dynamic passenger demand, we propose a new charging strategy: proactive partial charging. We design the p2Charging framework that employs a receding horizon optimization approach to coordinate the charging process and the dispatch process tightly and simultaneously with real-time multi-source data. The evaluation results show that p2Charging improves the ratio of unserved passengers by up to 83.2% on average and increases e-taxi utilization by up to 34.6% compared with ground truth and existing charging strategies. [ICDCS 2019]


We aim to coordinate  an  e-taxi  fleet  for  optimizing  charging  cost with both  conventional  and  renewable  energy  while maintaining the taxi service quality. We  propose  SAC,  an  e-taxi  fleet  coordination  framework to  dispatch  e-taxis  for  either  charging  or  serving passengers  under spatio-temporal  dynamics  of  renewable  energy  and passenger mobility. Our data-driven  evaluation  shows  that  our  solution significantly reduces the total reverse power flow per day by 94.8% while only reducing the number of served passengers by2.3% compared to the solution focusing on optimizing the e-taxi service quality. [CDC 2021, ACC 2022]



## Dynamic Integration of Heterogeneous Transportation Modes under Disruptions


With passenger trip data collected from a subway system, we analyze the degradation of service quality when the disruption happens to a subway line. We design a service framework called eRoute, which dynamically selects and coordinates heterogeneous mobile systems according to the characteristics of the disruptive events and mobile systems. We design a hierarchical Receding Horizon Control framework to adapt our solutions according to both current and estimated future passenger demand. The data-driven evaluation shows that compared to existing approaches with real-time data-driven features, our solution improves the ratio of served passengers per time interval by up to 11.5 times and reduces the average traveling time by up to 82.1%. [ICCPS 2018, TMC]


## Occupancy Patten Modeling and Prediction for Effective HVAC Control

With long-term occupant-count data collected from a commercial building, we develop models to capture occupancy dynamics and predict future occupancy patterns. We design an adaptive model predictive controller to minimize inefficient control actions according to different types of misprediction and occupancy states. Our control design provides probabilistic guarantees on the control cost under occupancy prediction uncertainty. Our evaluation shows that the proposed solution reduces energy consumption by 29.5% while improving the average weighted occupant comfort by 86.7% in Predicted Mean Vote (PMV) over the fixed schedule strategy. [IoTDI 2020]


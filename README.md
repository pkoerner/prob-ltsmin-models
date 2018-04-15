# prob-ltsmin-models
 B and Event-B models used to benchmark the integration of LTSmin and ProB.



## Models


### `CAN_BUS_tlc.mch` (aka CAN Bus)

This is a model of a CAN (Controller Area Network) bus which are usually used in cars. It was written by John Colley.

### `Core.mch`

This model is a part of an Access Controller and was submitted in a bug report by Nghi Huynh and Marc Frappier (see https://probjira.atlassian.net/projects/PROB/issues/PROB-320?)

### `earley_2.eventb` (aka Earley Parser)

This is a model of the earley parsing algorithm, written by Jean-Raymond Abrial, with the help of Dominique Cansell. The purpose was to formally derive the Earley parsing algorithm in Event-B and to establish its correctness. The model contains four refinement steps and very complicated guards. Every event corresponds to a step in the parsing algorithm. The purpose was to animate the model for a particular grammar and to reproduce the sequence in http://en.wikipedia.org/wiki/Earley_parser.


### `SetLawsNat.mch` (aka Set Laws)

This model is a toy example used to test that sets implemented in ProB are obeying the mathematical laws of sets.


### `Simpson_Four_Slot.mch` (aka Four Slot)

A model of Simpson's four slot algorithm. This B model only represents the individual steps of the algorithm. It is intended to be used in conjunction with a CSP model to describe the sequencing of the steps. Here, the B model on its own is model checked.


### `ModeProtocolMachine_mch.eventb` (aka Mode Protocol)

The model was developed by Space Systems Finland as part of a Distributed System for Attitude and Orbit Control for a Single Spacecraft (DSAOCSS) System. The model was a part of the case study within the EU Project DEPLOY.

See also: 

- Dubravka Ilic, Linas Laibinis, Timo Latvala, Elena Troubitsyna, and Kimmo Varpaaniemi. Deployment in the Space Sector. In Industrial Deployment of System Engineering Methods, pages 45–62. Springer, 2013.
- Dubravka Ilic, Timo Latvala, Pauli Väisänen, Kimmo Varpaaniemi, Linas Laibinis, and Elena Troubitsyna. DEPLOY Deliverable D20 D3.1 - Report on Pilot Deployment in the Space Sector. Technical report, 2010. Available at http://www.deploy-project.eu/html/deliverables.html.
- Dubravka Ilic, Timo Latvala, Laura Nummila, Tuomas Räsänen, Pauli Väisänen, Kimmo Varpaaniemi, Linas Laibinis, Yuliya Prokhorova, Elena Troubitsyna, Alexei Iliasov, Alexander Romanovsky, Michael Butler, Asieh Salehi Fathabadi, Abdolbaghi Rezazadeh, Jean-Christophe Deprez, Renaud De Landtsheer, and Christophe Ponsard. DEPLOY Deliverable D39 D3.2 - Report on Enhanced Deployment in the Space Sector. Technical report, 2011. Available at http://www.deploy-project.eu/html/deliverables.html.

### `obsw_M001.eventb` (aka Mercury Orbiter)
This model was also developed by Space Systems Finland.
It models part of a system of a Mercury Planetary Orbiter.

See also: 

- Dubravka Ilic, Linas Laibinis, Timo Latvala, Elena Troubitsyna, and Kimmo Varpaaniemi. Deployment in the Space Sector. In Industrial Deployment of System Engineering Methods, pages 45–62. Springer, 2013.
- Dubravka Ilic, Timo Latvala, Pauli Väisänen, Kimmo Varpaaniemi, Linas Laibinis, and Elena Troubitsyna. DEPLOY Deliverable D20 D3.1 - Report on Pilot Deployment in the Space Sector. Technical report, 2010. Available at http://www.deploy-project.eu/html/deliverables.html.
- Dubravka Ilic, Timo Latvala, Laura Nummila, Tuomas Räsänen, Pauli Väisänen, Kimmo Varpaaniemi, Linas Laibinis, Yuliya Prokhorova, Elena Troubitsyna, Alexei Iliasov, Alexander Romanovsky, Michael Butler, Asieh Salehi Fathabadi, Abdolbaghi Rezazadeh, Jean-Christophe Deprez, Renaud De Landtsheer, and Christophe Ponsard. DEPLOY Deliverable D39 D3.2 - Report on Enhanced Deployment in the Space Sector. Technical report, 2011. Available at http://www.deploy-project.eu/html/deliverables.html.


### `Ref5_Switch_mch.eventb` (aka Landing Gear)

This machine is the fifth refinement step of a model of a landing gear. The landing gear system was a case study at ABZ 2014. 

See also:
- D. Hansen, L. Ladenberger, H. Wiegard, J. Bendisposto, and M. Leuschel. Validation of the ABZ Landing Gear System Using ProB. Springer, 2014.


### `rether.eventb` (aka RETHER protocol)

This is a model of a real time ethernet protocol. The Event-B model is a translation by Marc Büngener of a model for DiVinE.

See also:
- Chitra Venkatramani and Tzicker Chiueh. Design, Implementation, and Evaluation of a Software-based Real-time Ethernet Protocol. SIGCOMM Comput. Commun. Rev., 25(4):27–37, October 1995.


### `Train_1_beebook_TLC.mch` (aka Train)

This interlocking system is a variation of the model from Abrial's book. The model has a reduced state space, which was achieved by manually applying a partial order reduction.

See also:
- Jean-Raymond Abrial. Modeling in Event-B: System and Software Engineering. Cambridge University Press, New York, NY, USA, 1st edition, 2010.

### `Train1_Lukas_POR.mch` (aka Train (reduced))

This is the first level refinement of the railway interlocking used in Train.
It uses a simplified topology and routes are released immediately when all blocks are free (to reduce the state space).

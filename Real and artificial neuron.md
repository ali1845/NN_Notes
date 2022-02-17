# Real and Artificial Neurons

## Structure of real neuron

###### Cell Body/Soma:
It contains all the organelles or subcellular components of the cell, which are present mostly in all of the cells. i.e. nucleus, mitochondria, etc.

Neurons are different from any other usuall cell because it functions as a *signal proceesing device*.

###### Membrane/surface of the Soma:
Neuron's membrane is covered with set of fibers which are emanating from the soma. These fibers are resposible for electrochemical processes. The one which is resposible for transmitting signals is **Axon** and all the other fibers are **Dentrites**.

###### Axon
Acting as the output of the neuron, it transmits signals to other neurons. Axon usually have a branch of **collaterals**, through which it may contact many other neurons.

###### Dentrites
Acting as the input of the neuron, they transmits signals from other neurons to the cell body.

###### Afferent & Effernt
**Afferent** are the neurons that supply input to a respective neuron.

**Effernt** is the axonal out of the neuron, which supply output to other neurons.

Afferent axons innervate with a perticular neuron by contacting the dentrites of the neuron at the junction called **Synapses**.

###### Synapses
It is the junction of the axon from where it contact other neurons. At synapses, the end of the afferent axon, **postsynaptic axon terminal** which get really close to the dentritic surface, **postsynaptic membrane**. The gap between the two surface, called **synaptic cleft**, is approximatly 20nm (2x10^8).

## Neurons acting as a Signal proceesing device
- Neural membrane maintains an electrical imbalance of the negatively and positively chaged ions, at the state of equilibrium.
- Neural membrane is negatively polarized from the inside and keeping the outside positively polarized.
- This separation of positive and negative charges generates a *potential difference* across the membrane, approximatly of 70mV.
- Thus, neural membrane support electrical signals if the *membrane potential* or the state of polarization is changed.
- Signals that propagate along axon is called **action potential**.
- The graph of each signal that propagate has the same, sharp pulse-like spikes, shape.
- Neurons usually have their axons sheathed in a fatty substance, called myelin, which supports rapid conduction of action potential.

#### Passage of signals through a single neuron

1. A large number of very small vesicles contain chemical substance, **neurotransmitter**,
2. When Action potential reaches the terminal of afferent axon, these vesciles migrate to **presynaptic membrane**,
3. Neurotransmitter are released accross the **synaptic clift**, through presynaptic membrane,
4. Transmitters chemically binds with the reciptor sites at **postsynaptic membrane**,
5. Electrochemical process is initiatied and it changes the polarization state of the membrane, this generates a **postsynaptic potential (PSP)**.
6. There are two things PSP can do;
   - **Depolarizing the membrane** from negative resting state to 0 volts. Making PSPs positive, which encourage neural signals and they are called excitatory PSPs or **EPSPs**.
   - **Hyperpolarizing the membrane** to an even higher negative potential and are called inhabitory PSPs or **IPSPs**.
   - All action potentials have the same high value and characteristics, but PSPs can have a range of values depending on the efficiency of the **synapses** in utilizing the chemical transmitter to produce an electrical signal.
7. PSP spread out through dentrites towards the cell body and reaches **axon hillock** -> where axon joins soma.
8. Just like these, there are thousands of other synaptic events occuring in the neuron parrallely. All of them are jumbling up at the axon hillock where they all are summed together to produce a **resultant membrane potential**.
9. PSPs are integrated by the neuron over space and time both.
   - PSPs usually exist for some period of time and then it decays. So even if two PSPs arrived slightly out of synchrony they may still affect the summation process.
   - But even if two synaptic events concurrently and take place in synchrony they may not effect the summation process, as by the time reaching axon hillock it may have decayed.
10. At the axons hillock the **sum of all PSPs** will result in **generating an action potential** if the thershold is increased by -50mV.
11. The generated action potential is then propagate through the axon, reaching axon terminal and shower the neighbouring neuron with synaptic events.
12. Once an action potential has been produce there is a short **refactory period**. In which all the ionic metabolites have been depleted. So there can be no other initiation of action potential no matter the value of the membrane potential.

#### Examine Real neuron to create an Artificial neuron

1. Action potential is resposible for signal transmission in a neuron, which has all or nothing, 0 or 1 property.
2. Action potential strikes the input or at synapse which generates a PSP which is variable and depends on the physiochemical properties of the synapse.
3. PSPs can be inhabitory (-ive) or excitatory(+ive).
4. PSPs reach axon hillock where they are summed up to generate membrane potential.
5. If this potential exceeds the threshold, action potential is generated which propagate through axon.

---

## Artificial Neurons, the TLU
Modeling some of the characteristics that are mentioned above,

###### All or nothing
- It is the characteristics of action potential to have a value or don't have any value. There os no thing such as half action potential.
- Hence, it can be characterized as two-valued signal. Which can only be either **binary**, 0 or 1, or **boolean**, True or false.
- e.g. If a node is reciving `n` input signals, `x1, x2, ... xn` then these can only have values either 0 or 1.

###### Excitatory and Inhabitory actions
- We have `n` weights, `w1, w2, ..., wn` and we will form an `n` products, `w1.x1, w2.x2, ..., wn.xn`.
- Each product is a representation of PSP, which can be either positive(excitatory) or negative(inhabitory), depending on the sign of the weight.
- To produce the activation, the products will simply be added together,
      a= w1x1 + w2x2 + ... + wnxn
    e.g.
    Lets have five-input unit with weights;

    `w1 = 0.5, w2 = 1.0, w3 = -1.0, w4 = -0.5, w5 = 1.2`

    

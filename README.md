# ece486-lab-3--digital-simulation-of-a-closed-loop-system-solved
**TO GET THIS SOLUTION VISIT:** [ECE486 Lab 3- Digital Simulation of a Closed Loop System Solved](https://mantutor.com/product/ece486-lab-3-digital-simulation-of-a-closed-loop-system-solved/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;115010&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ECE486 Lab 3- Digital Simulation of a Closed Loop System Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Scope and Objective

1. Study a closed loop system for speed control of a belt driven system through digital simulation <img draggable="false" role="img" class="emoji" alt="◼" src="https://s.w.org/images/core/emoji/15.1.0/svg/25fc.svg">Model the system of a magnetic tape drive such as a cassette player as an example

2. Implement different controllers and evaluated their effectiveness for different design objectives <img draggable="false" role="img" class="emoji" alt="◼" src="https://s.w.org/images/core/emoji/15.1.0/svg/25fc.svg">Achieving disturbance rejection and a smooth step response simultaneously

Introduction

Our previous lab activities have so far equipped us with the skills for modeling and analysis of the system dynamics. We will now move towards designing solutions that achieve specific desired outcome in terms of system(dynamics) behavior of interest. A closed loop system with feedback control, as you have seen in lectures, could facilitate such design goals.

In this lab we will look at the example in controlling the speed of a belt driven system using the cassette player as an example.

Reading

G. F. Franklin, et al., Feedback Control of Dynamic Systems, 3rd or 4th Ed., Sec. 4.1, 4.1.1. These pages can be found in Course Blackboard. In 7th or 6th Ed., see Sec. 4.2.2 for distance rejection.

The following contents are from ECE486 Control Systems Lab Manual,

Lab Session 3

Digital Simulation of a Closed Loop System

In this experiment Simulink is used to study a closed loop system for speed control of a magnetic tape drive such as a cassette player. You will compare different controllers for their effectiveness in simultaneously accomplishing disturbance rejection and a smooth step response.

Z Preparation Y

Readings:

. G. F. Franklin, et al., Feedback Control of Dynamic Systems, 3rd or 4th Ed., Sec. 4.1, 4.1.1. These pages are copied for you and attached at the end of this manual. In 7th or 6th Ed., see Sec. 4.2.2 for distance rejection.

Prelab:

Modeling: A diagram of the system is shown below

Figure3.1. : Closed-Loop System with Unity Feedback.

The tape dynamics are modeled as a rotational mass-damper system:

Jω˙(t) + Bω(t) = τ(t) + τd(t),

where J = 0.25[kg · m2], B = 3[N · m · s]. The torque motor transfer function is determined by an open-loop test with the motor detached from the system. A one-volt step is applied (zero initial conditions), and the resulting motor torque is

τ(t) = 5(1 − e−3t), t &gt; 0.

The amplifier is a non-inverting gain, K. It is assumed that the tape speed sensor (tachometer) dynamics can be neglected.

24 3 Digital Simulation of a Closed Loop System

Design: We want to have a closed loop system whose steady-state response from a disturbance is small, and whose step response from a reference input has low overshoot.

(a) Obtain an all-integrator block diagram for the system in figure 3.1. Show theintermediate variables (τ, v etc.). Note that the motor torque is the convolution of a step input with the motor’s transfer function.

(b) For the closed-loop system, find the transfer functions Ω(s)/Ωr(s) (with τd = 0) and Ω(s)/Td(s) (with ωr = 0). Use numerical values where given. (Hint: remember to make your lead coefficient 1.)

(c) For what values of K is the closed loop system stable?

(e) Express the desired value of Kr, in terms of K, such that the steady-state output speed for a unit step in ωr is 1. (τd = 0)

(f) Using the minimum value of K that you found in (d), what are the values of the closed loop ζ and ωn? Consider the anticipated response ω(t) to a step at ωr (τd = 0). What will be the expected ts, tr, and Mp? Use the equations on page 13.

(g) Controller 2: Suppose, alternatively, that K is selected to produce a low overshoot (ζ &gt; 0.75). Find the range of K that meets this specification. If K is selected such that ζ = 0.75, what will be the steady-state disturbance response to a unit step? What Mp do we achieve? Can we achieve both our desired disturbance rejection and our desired overshoot?

(h) Controller 3: To improve the response, suppose we add derivative feedback (measured by an accelerometer in this case) as shown:

Figure3.2. : Closed-Loop System with Derivative Feedback.

Compute again the new closed-loop transfer functions Ω(s)/Ωr(s) (with τd = 0) and Ω(s)/Td(s) (with ωr = 0). Give the ranges of K and K·Kd for which the closed-loop system is stable.

25

f Laboratory Exercise f

1. Develop an all-integrator Simulink block-diagram for the three closed-loop control systems. It is a good simulation practice to retain explicitly in the simulation the various subsystems – actuator, plant, amplifiers, etc. Your diagram should do so, and you should label the inputs and outputs, ω, τ, v, e, of the subsystems. It is possible to make only one diagram, and simply use Matlab variables in the Simulink blocks for the different cases. Do not use differentiators in your diagram. Instead, route the required states around the integrators. See appendix A, section IV-c for an example of this.

2. Obtain and print the following time responses for each of the three controllers:

• ω(t) for the disturbance response to a unit step in τd (ωr = 0). For comparison, overlay and label the plots for the different controllers.

• ω(t) for the reference response to a unit step in ωr (τd = 0). Remember to use the appropriate value of Kr for each controller. Overlay again for comparison. You should end up with six graphs on two plots.

V Report V

1. Include your prelab calculated values and experimental data (time responses) obtained. Compare the values of Mp, tr, and ts as calculated in the prelab with the values obtained from Matlab. Which controllers met the specifications (steady state disturbance response 6 0.01 rad/s and ζ &gt; 0.75)?

2. For the system in Figure 3.1, derive the relationship between the steady-stateerror (ess = ωr − ω) and the natural frequency, ωn. Consider the error as a function of both ωr and τd, when both are step inputs. Since the system is linear, superposition allows the two components of ess to be calculated separately and then summed.

3. For controller 3, solve for ζ and ωn in terms of the gains K and Kd. From these equations, sketch a plot of how the pole locations change as Kd &gt; 0 increases in value.

26 3 Digital Simulation of a Closed Loop System

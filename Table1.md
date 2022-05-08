## From values to criteria and their manifestations

| Value       | Criteria  | Manifestations|
| ----------- |---------- | --------------
| Privacy     | 1. **Consent for data usage** ([[1]](#GDPR2018), [[2]](#fjeld2020), [[3]](#krafft2020))  <br> 2. **Data protection** ([[2]](#fjeld2020),[[3]](#krafft2020),[[4]](#floridi2019))<br> 3. **Control over data / ability to restrict processing** ([[1]](#GDPR2018), [[2]](#fjeld2020))<br> 4. **Right to rectification** ([[1]](#GDPR2018), [[2]](#fjeld2020), [[3]](#krafft2020)) <br> 5. **Right to erase the data** ([[1]](#GDPR2018), [[2]](#fjeld2020), [[3]](#krafft2020))<br> 6. **Right of access by data subject, data agency** ([[1]](#GDPR2018), [[5]](#IEEE2019)) | - <span style="color:orange">Written declaration of consent</span>([[1]](#GDPR2018)) <br> - <span style="color:orange">Description of what data is collected</span>([[6]](#mehldau2007)) <br> - <span style="color:orange">Description of how data is handled</span> ([[6]](#mehldau2007)) <br> - <span style="color:orange">Purpose statement of data collection</span> ([[6]](#mehldau2007)) <br> - <span style="color:orange">Statement of how long the data is kept</span> ([[6]](#mehldau2007)) <br> - <span style="color:olive">For and submission mechanisms to object data collection and to make complaints</span> ([[7]](#blazevic2021)) <br> - <span style="color:olive">Obfuscation of data</span> ([[3]](#krafft2020))                                           
| Security    | 1. **Resilience to attacks**: protection of privacy ([[8]](#microsoftai2018), [[9]](#hidalgo2021), [[10]](#wachter2019)), vulnerabilities, fallback plans ([[2]](#fjeld2020), [[3]](#krafft2020), [[11]](#morley2020), [[12]](#googleai2018)) <br>2. **Predictability** ([[2]](#fjeld2020), [[3]](#krafft2020), [[13]](#europeancommissionEthicsAI2019)) <br> 3. **Robustness / reliability**: prevent manipulation ([[3]](#krafft2020)) | AGAINST INTEGRITY THREATS ([[14]](#xiong2021)): <br> Training time ([[14]](#xiong2021)). Ex.:<br><span style="color:olive"> -Data sanitization[^1] ([[15]](#biggio2018), [[16]](#cretu2008))<br> -Robust learning[^2] ([[15]](#biggio2018), [[17]](#globerson2006))<br></span><br> Prediction time ([[14]](#xiong2021)):<br> <span style="color:olive"> - Model enhancement ([[15]](#biggio2018), [[18]](#lyu2015), [[19]](#goodfellow2014), [[20]](#papernot2016))<br> - Adversarial learning[^3]<br> - Gradient masking[^4]<br> - Defensive Distillation[^5]</span> <br><br> AGAINST PRIVACY THREATS ([[14]](#xiong2021)): <br> Mitigation techniques ([[21]](#nasr2018)):<br> <span style="color:olive"> - Restrict prediction vector to top k classes[^6] ([[22]](#shokri2017))<br> - Coarsen the precision of the prediction vector[^7] ([[22]](#shokri2017))<br> - Increase entropy of the prediction vector[^8] ([[22]](#shokri2017))<br> - Use regularization[^9]([[22]](#shokri2017), [[23]](#kaya2020))<br></span>  <br>Differential privacy mechanisms ([[21]](#nasr2018)): <br>    <span style="color:olive"> - Differential privacy[^10] ([[24]](#ye2021), [[25]](#dwork2006)). Ex.:<br> - Adversarial regularization[^11] ([[21]](#nasr2018))<br> - MemGuard[^12] ([[26]](#jia2019)</span> 
| Performance | 1. **Correctness of predictions** ([[2]](#fjeld2020), [[13]](#europeancommissionEthicsAI2019), [[27]](#bihrane2021)) <br> 2. **Memory efficiency** ([[3]](#krafft2020)), [[27]](#bihrane2021))<br> 3. **Training efficiency** ([[27]](#bihrane2021)) <br> 4. **Energy efficiency** ([[3]](#krafft2020)), [[27]](#bihrane2021)) <br> 5. **Data efficiency** ([[27]](#bihrane2021))  |   - <span style="color:magenta">Accuracy ([[28]](#mitchell2019), [[29]](#wexler2019))</span> <br> - <span style="color:magenta">False Positive and Negative rates ([[28]](#mitchell2019), [[29]](#wexler2019))</span> <br> - <span style="color:magenta">False Discovery and Omission rates ([[28]](#mitchell2019))</span> <br> - <span style="color:magenta">Mean and median error ([[29]](#wexler2019))</span> <br> - <span style="color:magenta">R2 score ([[30]](#bird2020))</span> <br> - <span style="color:magenta">Precision and recall rates ([[29]](#wexler2019))</span><br> - <span style="color:magenta">Area under ROC curve (AUC) ([[30]](#bird2020))</span> <br> - <span style="color:magenta">Estimation of energy consumption through ([[31]](#garciamartin2019)):<br></span> <span style="color:black"> - performance counters<br> - simulation<br> - instruction- or architecture-level estimations<br> - real-time estimation</span>- <span style="color:magenta">Estimation of GPU memory consumption ([[32]](#gao2020), [[33]](#mahendran2021))</span> <br> - <span style="color:magenta">Wall-clock training time ([[34]](#assran2020), [[35]](#dalton2020))</span>  
|Respect for public interest | 1. **Desirability of technology** ([[36]](#chasalow2021), [[37]](#abebe2020), [[38]](#keyes2019))<br> 2. **Benefit to society** ([[2]](#fjeld2020), [[4]](#floridi2019), [[11]](#morley2020), [[39]](#floridi2018))<br> 3. **Environmental impact** ([[3]](#krafft2020), [[40]](#bender2021)) | - <span style="color:olive">Diverse and inclusive forum for discussion ([[2]](#fjeld2020), [[41]](#frenchminister2019))</span> <br> - <span style="color:orange">Measure of social and environmental impact ([[11]](#morley2020), [[40]](#bender2021)), [[42]](#raji2020))</span> 
|Fairness| 1. **Individual fairness**[^13] ([[25]](#dwork2006), [[43]](#mehrabi2021), [[44]](#barredoarrieta2020), [[45]](#kusner2017))<br> 2. **Demographic parity**[^14] ([[9]](#hidalgo2021), [[25]](#dwork2006), [[43]](#mehrabi2021),[[44]](#barredoarrieta2020), [[45]](#kusner2017), [[46]](#harrison2020), [[47]](#srivastava2019), [[48]](#kearns2018), [[49]](#verma2018))<br> 3. **Conditional statistical parity**[^15] ([[43]](#mehrabi2021), [[49]](#verma2018))<br> 4. **Equality of opportunity**[^16]([[43]](#mehrabi2021), [[50]](#hardt2016), [[51]](#vanBerkel2021)) <br> 5. **Equalized odds**[^17] ([[43]](#mehrabi2021))<br> 6. **Treatment equality**[^18] ([[43]](#mehrabi2021), [[52]](#berk2017))<br> 7. **Test fairness**[^19] ([[43]](#mehrabi2021), [[49]](#verma2018), [[53]](#chouldechova2016))<br> 8. **Procedural fairness**[^20] ([[43]](#mehrabi2021), [[45]](#kusner2017), [[54]](#grgichlaca2018)) | - <span style="color:magenta">Accuracy across groups ([[11]](#morley2020), [[46]](#harrison2020), [[53]](#chouldechova2016), [[55]](#kleinberg2016))</span><br> - <span style="color:magenta">False positive and negative rates across groups ([[43]](#mehrabi2021), [[53]](#chouldechova2016), [[55]](#kleinberg2016), [[56]](#wang2020), [[57]](#saleiro2018))</span> <br> - <span style="color:magenta">False discovery and omission rates across groups ([[28]](#mitchell2019), [[57]](#saleiro2018))</span><br> - <span style="color:magenta">Pinned AUC ([[28]](#mitchell2019), [[58]](#dixon2018))</span><br> - <span style="color:olive">Debiasing algorithms ([[59]](#bellamy2018))</span><br> - <span style="color:olive">Election of protected classes based on user considerations ([[54]](#grgichlaca2018))</span> 
| Non-discrimination| 1. **Quality and integrity of data** ([[2]](#fjeld2020), [[9]](#hidalgo2021), [[11]](#morley2020), [[60]](#stuartgeiger2020), [[61]](#paullada2020)) <br> 2. **Inclusiveness in design** ([[2]](#fjeld2020), [[11]](#morley2020), [[13]](#europeancommissionEthicsAI2019))<br> 3. **Accessibility** ([[2]](#fjeld2020), [[3]](#krafft2020), [[11]](#morley2020), [[27]](#bihrane2021)) | - <span style="color:olive">Inclusive data generation process ([[3]](#krafft2020), [[11]](#morley2020), [[36]](#chasalow2021), [[60]](#stuartgeiger2020))</span> <br> - <span style="color:magenta">Analysis of data for potential biases, data quality assessment ([[2]](#fjeld2020),[[3]](#krafft2020), [[9]](#hidalgo2021), [[43]](#mehrabi2021), [[62]](#gebru2020))</span><br>- <span style="color:olive">Diversity of participant in development process ([[2]](#fjeld2020), [[3]](#krafft2020), [[63]](#lee2019), [[64]](#zhouWeb))</span><br> - <span style="color:olive">Access to code and technology to all ([[2]](#fjeld2020), [[3]](#krafft2020), [[11]](#morley2020), [[27]](#bihrane2021))</span>
| Transparency| 1. **Interpretability of data and models** ([[27]](#bihrane2021), [[65]](#royalsociety2019))<br> 2. **Enabling human oversight of operations** ([[2]](#fjeld2020), [[11]](#morley2020))<br>3. **Accessibility of data and algorithm** ([[2]](#fjeld2020), [[3]](#krafft2020), [[65]](#royalsociety2019))<br> 4. **Traceability** [[11]](#morley2020)<br>5. **Reproducibility** [[27]](#bihrane2021)| - <span style="color:orange">Description of data generation process ([[3]](#krafft2020), [[11]](#morley2020), [[36]](#chasalow2021), [[60]](#stuartgeiger2020), [[62]](#gebru2020), [[66]](#bender2018))</span><br> - <span style="color:orange">Disclosure of origin and properties of models and data ([[3]](#krafft2020), [[28]](#mitchell2019), [[65]](#royalsociety2019))</span><br> - <span style="color:olive">Open access to data and algorithms ([[2]](#fjeld2020), [[3]](#krafft2020), [[27]](#bihrane2021), [[65]](#royalsociety2019))</span><br> - <span style="color:orange">Notification of usage/interaction ([[2]](#fjeld2020))</span><br> - <span style="color:orange">Regular reporting ([[2]](#fjeld2020))</span>
|Explainability| 1. **Ability to understand AI systems and the decision reached** ([[4]](#floridi2019), [[13]](#europeancommissionEthicsAI2019), [[27]](#bihrane2021), [[39]](#floridi2018), [[65]](#royalsociety2019), [[67]](#OECD2019))<br> 2. **Traceability** ([[11]](#morley2020)) <br> 3. **Enable evaluation** ([[2]](#fjeld2020), [[11]](#morley2020)) | - <span style="color:olive">Interpretability by design ([[44]](#barredoarrieta2020))</span><br> - <span style="color:olive">Post-hoc explanations ([[44]](#barredoarrieta2020))</span>
|Contestability | 1. **Enable argumentation / negotiation against a decision** ([[2]](#fjeld2020), [[13]](#europeancommissionEthicsAI2019), [[65]](#royalsociety2019), [[68]](#balayn2021Edri), [[69]](#kyunglee2017), [[70]](#alfrink2020), [[71]](#kalluri2020), [[72]](#lyons2021)) <br> 2. **Citizen empowerment** ([[13]](#europeancommissionEthicsAI2019), [[68]](#balayn2021Edri), [[71]](#kalluri2020))| - <span style="color:orange">Information of who determines and what constitutes a contestable decision and who is accountable ([[72]](#lyons2021))</span><br> - <span style="color:orange">Determination of who can contest the decision (subject or representative) ([[72]](#lyons2021))</span><br> - <span style="color:orange">Indication of type of review in place ([[72]](#lyons2021))</span><br> - <span style="color:orange">Information regarding the contestability workflow ([[72]](#lyons2021))</span><br> - <span style="color:olive">Mechanisms for users to ask questions and record disagreements with system behavior ([[73]](#hirsch2017), [[74]](#mitra2021))</span>
| Human Control | 1. **User/collective influence** ([[27]](#bihrane2021), [[69]](#kyunglee2017)) <br> 2. **Human review of automated decision** ([[2]](#fjeld2020))<br> 3. **Choice of how and whether to delegate** ([[2]](#fjeld2020))| - <span style="color:olive">Continuous monitoring of system to intervene ([[2]](#fjeld2020), [[13]](#europeancommissionEthicsAI2019), [[75]](#teliaai2019))</span><br> - <span style="color:olive">Establishment levels of human discretion during the use of the system ([[8]](#microsoftai2018), [[13]](#europeancommissionEthicsAI2019))</span><br> - <span style="color:olive">Ability to override the decision made by the system ([[13]](#europeancommissionEthicsAI2019))</span>
| Human Agency| 1. **Respect for human autonomy** ([[2]](#fjeld2020), [[11]](#morley2020), [[13]](#europeancommissionEthicsAI2019))<br> 2. **Power to decide. Ability to make informed autonomous decision** ([[13]](#europeancommissionEthicsAI2019), [[27]](#bihrane2021))<br> 3. **Ability to opt out of an automated decision** ([[2]](#fjeld2020), [[13]](#europeancommissionEthicsAI2019))|- <span style="color:orange">Give knowledge and tools to comprehend and interact with AI system ([[13]](#europeancommissionEthicsAI2019))</span><br> - <span style="color:olive">Opportunity to self-assess the system ([[13]](#europeancommissionEthicsAI2019))</span>

Summary of the specific criteria that relate to each value considered in our ML assessment framework. These criteria are then translated into specific manifestations in the form of signifiers (orange), process-oriented practices (olive) or quantifiable indicators (magenta).

[Back to main page](index.md)

[^1]: It ensures data soundness by identifying abnormal input samples and by removing them ([[14]](#xiong2021))
[^2]: It ensures that algorithms are trained on statistically robust datasets, with little sensitivity to outliers ([[14]](#xiong2021))
[^3]: Adversarial samples are introduced to the training set ([[14]](#xiong2021))
[^4]: Input gradients are modified to enhance model robustness ([[14]](#xiong2021))
[^5]: The dimensionality of the network is reduced ([[14]](#xiong2021))
[^6]: Applicable when the number of classes is very large. Even if the model only outputs the most likely k classes, it will still be useful ([[22]](#shokri2017))
[^7]: It consists in rounding the classification probabilities down ([[22]](#shokri2017))
[^8]: Modification of  the softmax layer (in neural networks) to increase its normalizing temperature ([[22]](#shokri2017))
[^9]: Technique to avoid overfitting in ML that penalizes large parameters by adding a regularization factor $\lambda$ to the loss function ([[22]](#shokri2017))
[^10]: It prevents any adversary from distinguishing the predictions of a model when its training dataset is used compared to when other dataset is used ([[24]](#ye2021))
[^11]: Membership privacy is modeled as a min-max optimization problem, where a model is trained to achieve minimum loss of accuracy and maximum robustness against the strongest inference attack ([[21]](#nasr2018))
[^12]: Noise is added to the confidence vector of the attacker so as to mislead the attacker's classifier ([[26]](#jia2019))
[^13]: Similar individuals should be treated in a similar way. Diverging definitions state that: two individuals that are similar with respect to a common metric should receive the same outcome (*fairness through awareness*); or any protected attribute should not be used when making a decision (*fairness through unawareness*); or the outcome obtained by an individual should be the same if this individual belonged to a counterfactual world or group (*counterfactual fairness*) ([[43]](#mehrabi2021))
[^14]: The probability of getting a positive outcome should be the same whether the individual belongs to a protected group or not ([[43]](#mehrabi2021))
[^15]: Given a set of factors L, individuals belonging to the protected or unprotected group should have the same probability of getting a positive outcome ([[43]](#mehrabi2021))
[^16]: The probability for a person from class A (positive class) of getting a positive outcome, which should be the same regardless of the group (protected group or not) that the individual belongs to  ([[43]](#mehrabi2021))
[^17]: The probability for a person from class A (positive class) of getting a positive outcome and the probability for a person from class B (negative class) of getting a negative outcome should be the same ([[43]](#mehrabi2021))
[^18]: The ratio of false positives and negatives has to be the same for both groups ([[43]](#mehrabi2021))
[^19]: For any probability score S, the probability of correctly belonging to the positive class should be the same for both the protected and unprotected group ([[43]](#mehrabi2021))
[^20]: It deals with the fairness of the decision-making process that leads to the outcome in question ([[54]](#grgichlaca2018))

## References
<a id="GDPR2018">[1]</a> 
European Commission. 2018.
2018 reform of EU data protection rules. 
[https://ec.europa.eu/commission/sites/beta-political/files/data-protection-factsheet-changes_en.pdf](https://ec.europa.eu/commission/sites/beta-political/files/data-protection-factsheet-changes_en.pdf)

<a id="fjeld2020">[2]</a> 
Jessica Fjeld, Nele Achten, Hannah Hilligoss, Adam Nagy, Madhulika Srikumar. 2020.
Principled Artificial Intelligence: Mapping Consensus in Ethical and Rights-Based Approaches to Principles for AI. 
SSRN Electronic Journal (2020) [https://doi.org/10.2139/ssrn.3518482](https://doi.org/10.2139/ssrn.3518482)

<a id="krafft2020">[3]</a> 
AI Ethics Impact Group (AIEIG). 2020. 
From Principles to Practice An interdisciplinary framework to operationalise AI ethics. 
[https://www.ai-ethics-impact.org/resource/blob/1961130/c6db9894ee73aefa489d6249f5ee2b9f/aieig---report---download-hb-data.pdf](https://www.ai-ethics-impact.org/resource/blob/1961130/c6db9894ee73aefa489d6249f5ee2b9f/aieig---report---download-hb-data.pdf)

<a id="floridi2019">[4]</a> 
Luciano Floridi. 2019. 
Translating Principles into Practices of Digital Ethics: Five Risks of Being Unethical. 
Philosophy & Technology 32, 2 (6 2019). [https://doi.org/10.1007/s13347-019-00354-x](https://doi.org/10.1007/s13347-019-00354-x)

<a id="IEEE2019">[5]</a> 
IEEE. 2019.
The IEEE Global Initiative on Ethics of Autonomous and Intelligent Systems.
Ethically Aligned Design: A Vision for Prioritizing Human Well-being with Autonomous and Intelligent Systems (first edition ed.).

<a id="mehldau2007">[6]</a> 
Matthias Mehldau. 2007.
Iconset for data-privacy declarations v 0.1.
Ethically Aligned Design: A Vision for Prioritizing Human Well-being with Autonomous and Intelligent Systems (first edition ed.).

<a id="blazevic2021">[7]</a> 
Alice Namuli Blazevic, Patrick Mugalula, and Andrew Wandera. 2021. 
Towards Operationalizing the Data Protection and Privacy Act 2020 Understanding the Draft Data Protection and Privacy Regulations. 
SSRN Electronic Journal (2021). [https://doi.org/10.2139/ssrn.3776353](https://doi.org/10.2139/ssrn.3776353)

<a id="microsoftai2018">[8]</a> 
Microsoft. 2018. 
AI Principles.
[https://www.microsoft.com/en-us/ai/responsible-ai?activetab=pivot1%3aprimaryr6](https://www.microsoft.com/en-us/ai/responsible-ai?activetab=pivot1%3aprimaryr6)

<a id="hidalgo2021">[9]</a> 
César Hidalgo, Diana Orghian, Jordi Albo-Canals, Filipa de Almeida, and Natalia Martin. 2021. 
How Humans Judge Machines. 
MIT Press. [https://hal.archives-ouvertes.fr/hal-03058652](https://hal.archives-ouvertes.fr/hal-03058652)

<a id="wachter2019">[10]</a> 
Sandra Wachter and Brent Mittelstadt. 2019. 
Right to Reasonable Inferences: Re-Thinking Data Protection Law in the Age of Big Data and AI. 
Columbia Business Law Review 2 (2019), 494–620.

<a id="morley2020">[11]</a> 
Jessica Morley, Luciano Floridi, Libby Kinsey, and Anat Elhalal. 2020. 
From What to How: An Initial Review of Publicly Available AI Ethics Tools, Methods and Research to Translate Principles into Practices. 
Science and Engineering Ethics 26 (2020), 2141–2168. [https://doi.org/10.1007/s11948-019-00165-5](https://doi.org/10.1007/s11948-019-00165-5)

<a id="googleai2018">[12]</a> 
Google. 2018. 
AI at Google: Our Principles. 
[https://www.blog.google/technology/ai/ai-principles/](https://www.blog.google/technology/ai/ai-principles/)

<a id="europeancommissionEthicsAI2019">[13]</a> 
European Commission. 2019. 
Ethics guidelines for trustworthy AI. 
[https://www.aepd.es/sites/default/files/2019-12/ai-ethics-guidelines.pdf](https://www.aepd.es/sites/default/files/2019-12/ai-ethics-guidelines.pdf)

<a id="xiong2021">[14]</a> 
Pulei Xiong, Scott Buffett, Shahrear Iqbal, Philippe Lamontagne, Mohammad Mamun, and Heather Molyneaux. 2021. 
Towards a Robust and Trustworthy Machine Learning System Development. (1 2021).

<a id="biggio2018">[15]</a> 
Battista Biggio and Fabio Roli. 2018. 
Wild patterns: Ten years after the rise of adversarial machine learning. 
Pattern Recognition 84 (12 2018), 317–331. [https://doi.org/10.1016/j.patcog.2018.07.023](https://doi.org/10.1016/j.patcog.2018.07.023)

<a id="cretu2008">[16]</a> 
Gabriela F. Cretu, Angelos Stavrou, Michael E. Locasto, Salvatore J. Stolfo, and Angelos D. Keromytis. 2008. 
Casting out Demons: Sanitizing Training Data for Anomaly Sensors.
In 2008 IEEE Symposiumon Security and Privacy (sp2008).IEEE,81–95. [https://doi.org/10.1109/SP.2008.11](https://doi.org/10.1109/SP.2008.11)

<a id="globerson2006">[17]</a> 
Amir Globerson and Sam Roweis. 2006. 
Nightmare at test time. 
In Proceedings of the 23rd international conference on Machine learning - ICML ’06. ACMPress, New York, NewYork, USA, 353–360. [https://doi.org/10.1145/1143844.1143889](https://doi.org/10.1145/1143844.1143889)

<a id="lyu2015">[18]</a> 
Chunchuan Lyu, Kaizhu Huang, and Hai-Ning Liang. 2015. 
A Unified Gradient Regularization Family for Adversarial Examples. 
In 2015 IEEE International Conference on Data Mining.IEEE,301–309. [https://doi.org/10.1109/ICDM.2015.84](https://doi.org/10.1109/ICDM.2015.84)

<a id="goodfellow2014">[19]</a> 
Ian J. Goodfellow, Jonathon Shlens, and Christian Szegedy. 2014. 
Explaining and Harnessing Adversarial Examples. (12 2014).

<a id="papernot2016">[20]</a> 
Nicolas Papernot, Patrick McDaniel, Xi Wu, Somesh Jha, and Ananthram Swami. 2016. 
Distillation as a Defense to Adversarial Perturbations Against Deep Neural Networks. 
In 2016 IEEE Symposium on Security and Privacy (SP). IEEE, 582–597. [https://doi.org/10.1109/SP.2016.41](https://doi.org/10.1109/SP.2016.41)

<a id="nasr2018">[21]</a> 
Milad Nasr, Reza Shokri, and Amir Houmansadr. 2018. 
Machine Learning with Membership Privacy using Adversarial Regularization. (7 2018).

<a id="shokri2017">[22]</a> 
Reza Shokri, Marco Stronati, Congzheng Song, and Vitaly Shmatikov. 2016. 
Membership Inference Attacks against Machine Learning Models. (10 2016).

<a id="kaya2020">[23]</a> 
Yigitcan Kaya, Sanghyun Hong, and Tudor Dumitras. 2020. 
On the Effectiveness of Regularization Against Membership Inference Attacks. (6 2020).

<a id="ye2021">[24]</a> 
Jiayuan Ye, Aadyaa Maddi, Sasi Kumar Murakonda, and Reza Shokri. 2021. 
Enhanced Membership Inference Attacks against Machine Learning Models. (11 2021).

<a id="dwork2006">[25]</a> 
Cynthia Dwork, Frank McSherry, Kobbi Nissim, and Adam Smith. 2006. 
Calibrating Noise to Sensitivity in Private Data Analysis. 265–284.
[https://doi.org/10.1007/11681878_14](https://doi.org/10.1007/11681878_14)

<a id="jia2019">[26]</a> 
Jinyuan Jia, Ahmed Salem, Michael Backes, Yang Zhang, and Neil Zhenqiang Gong. 2019. 
MemGuard: Defending against Black-Box Membership Inference Attacks via Adversarial Examples. (9 2019).

<a id="bihrane2021">[27]</a> 
Abeba Birhane, Pratyusha Kalluri, Dallas Card, William Agnew, Ravit Dotan, and Michelle Bao. 2021. 
The Values Encoded in Machine Learning Research. (6 2021).

<a id="mitchell2019">[28]</a> 
Margaret Mitchell, Simone Wu, Andrew Zaldivar, Parker Barnes, Lucy Vasserman, Ben Hutchinson, Elena Spitzer, Inioluwa Deborah Raji, and Timnit Gebru. 2018. 
Model Cards for Model Reporting. (10 2018). [https://doi.org/10.1145/3287560.3287596](https://doi.org/10.1145/3287560.3287596)

<a id="wexler2019">[29]</a> 
James Wexler, Mahima Pushkarna, Tolga Bolukbasi, Martin Wattenberg, Fernanda Viegas, and Jimbo Wilson. 2019. 
The What-If Tool: Interactive Probing of Machine Learning Models.(7 2019). [https://doi.org/10.1109/TVCG.2019.2934619](https://doi.org/10.1109/TVCG.2019.2934619)

<a id="bird2020">[30]</a> 
Sarah Bird, Miro Dudík, Richard Edgar, Brandon Horn, Roman Lutz, Vanessa Milan, Mehrnoosh Sameki, Hanna Wallach, and Kath- leen Walker. 2020. 
Fairlearn: A toolkit for assessing and improving fairness in AI. 
Technical Report MSR-TR-2020-32. Microsoft. [https://www.microsoft.com/en-us/research/publication/fairlearn-a-toolkit-for-assessing-and-improving-fairness-in-ai/](https://www.microsoft.com/en-us/research/publication/fairlearn-a-toolkit-for-assessing-and-improving-fairness-in-ai/)

<a id="garciamartin2019">[31]</a> 
Eva García-Martín, Crefeda Faviola Rodrigues, Graham Riley, and Håkan Grahn. 2019. 
Estimation of energy consumption in machine learning. 
J.Parallel and Distrib.Comput. 134(12 2019),75–88. [https://doi.org/10.1016/j.jpdc.2019.07.007](https://doi.org/10.1016/j.jpdc.2019.07.007)

<a id="gao2020">[32]</a> 
Yanjie Gao, Yu Liu, Hongyu Zhang, Zhengxian Li, Yonghao Zhu, Haoxiang Lin, and Mao Yang. 2020. 
Estimating GPU memory consumption of deep learning models. 
In Proceedings of the 28th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering. ACM, NewYork, NY, USA, 1342–1352. [https://doi.org/10.1145/3368089.3417050](https://doi.org/10.1145/3368089.3417050)

<a id="mahendran2021">[33]</a> 
N. Mahendran. 2021. 
Analysis of memory consumption by neural networks based on hyperparameters. (10 2021).

<a id="assran2020">[34]</a> 
Mahmoud Assran, Joshua Romoff, Nicolas Ballas, Joelle Pineau, and Michael Rabbat. 2019. 
Gossip-based Actor-Learner Architectures for Deep Reinforcement Learning. (6 2019).

<a id="dalton2020">[35]</a> 
Steven Dalton, Iuri Frosio, and Michael Garland. 2019. 
Accelerating Reinforcement Learning through GPU Atari Emulation. (7 2019).

<a id="chasalow2021">[36]</a> 
Kyla Chasalow and Karen Levy. 2021. 
Representativeness in Statistics, Politics, and Machine Learning. 
In Proceedings of the 2021 ACM Conference on Fairness, Accountability, and Transparency (FAccT ’21). Association for Computing Machinery, New York, NY, USA, 77–89. [https://doi.org/10.1145/3442188.3445872](https://doi.org/10.1145/3442188.3445872)

<a id="abebe2020">[37]</a> 
Rediet Abebe, Solon Barocas, Jon Kleinberg, Karen Levy, Manish Raghavan, and David G. Robinson. 2020. 
Roles for computing in so- cial change. 
In Proceedings of the 2020 Conference on Fairness, Accountability, and Transparency. ACM, New York, NY, USA, 252–260. [https://doi.org/10.1145/3351095.3372871](https://doi.org/10.1145/3351095.3372871)

<a id="keyes2019">[38]</a> 
Os Keyes, Jevan Hutson, and Meredith Durbin. 2019. 
A Mulching Proposal: Analysing and Improving an Algorithmic System for Turning the Elderly into High-Nutrient Slurry. 
In Extended Abstracts of the 2019 CHI Conference on Human Factors in Computing Systems (CHI EA ’19). Association for Computing Machinery, New York, NY, USA,1–11. [https://doi.org/10.1145/3290607.3310433](https://doi.org/10.1145/3290607.3310433)

<a id="floridi2018">[39]</a> 
Luciano Floridi, Josh Cowls, Monica Beltrametti, Raja Chatila, Patrice Chazerand, Virginia Dignum, Christoph Luetge, Robert Madelin, Ugo Pagallo, Francesca Rossi, Burkhard Schafer, Peggy Valcke, and Effy Vayena. 2018. 
AI4People—An Ethical Framework for a Good AI Society: Opportunities, Risks, Principles, and Recommendations. 
Minds and Machines 28, 4 (12 2018). 

<a id="bender2021">[40]</a> 
Emily M Bender, Timnit Gebru, Angelina McMillan-Major, and Shmargaret Shmitchell. 2021. 
On the Dangers of Stochastic Parrots: Can Language Models Be Too Big?. 
In Proceedings of the 2021 ACM Conference on Fairness, Accountability, and Transparency (FAccT ’21). Association for Computing Machinery,NewYork,NY,USA,610–623. [https://doi.org/10.1145/3442188.3445922](https://doi.org/10.1145/3442188.3445922)

<a id="frenchminister2019">[41]</a> 
Mission assigned by the French Prime Minister. 2019. 
For a Meaningful Artificial Intelligence: Toward a French and European Strategy. [https://www.aiforhumanity.fr/pdfs/MissionVillani_Report_ENG-VF.pdf](https://www.aiforhumanity.fr/pdfs/MissionVillani_Report_ENG-VF.pdf)

<a id="raji2020">[42]</a> 
Inioluwa Deborah Raji, Andrew Smart, Rebecca N. White, Margaret Mitchell, Timnit Gebru, Ben Hutchinson, Jamila Smith-Loud, Daniel Theron, and Parker Barnes. 2020. 
Closing the AI accountability gap. 
In Proceedings of the 2020 Conference on Fairness, Accountability, and Transparency. ACM,NewYork,NY,USA,33–44. [https://doi.org/10.1145/3351095.3372873](https://doi.org/10.1145/3351095.3372873)

<a id="mehrabi2021">[43]</a> 
Ninareh Mehrabi, Fred Morstatter, Nripsuta Saxena, Kristina Lerman, and Aram Galstyan. 2021. 
A Survey on Bias and Fairness in Machine Learning. 
ACM Comput. Surv. 54, 6 (7 2021). [https://doi.org/10.1145/3457607](https://doi.org/10.1145/3457607)

<a id="barredoarrieta2020">[44]</a> 
Alejandro Barredo Arrieta, Natalia Díaz-Rodríguez, Javier Del Ser, Adrien Bennetot, Siham Tabik, Alberto Barbado, Salvador Garcia, Sergio Gil-Lopez, Daniel Molina, Richard Benjamins, Raja Chatila, and Francisco Herrera. 2020. 
Explainable Artificial Intelligence (XAI): Concepts, taxonomies, opportunities and challenges toward responsible AI. 
Information Fusion 58 (6 2020), 82–115. [https://doi.org/10.1016/J.INFFUS.2019.12.012](https://doi.org/10.1016/J.INFFUS.2019.12.012)

<a id="kusner2017">[45]</a> 
Matt J Kusner, Joshua Loftus, Chris Russell, and Ricardo Silva. 2017. 
Counterfactual Fairness. 
In Advances in Neural Information Processing Systems, I Guyon, U V Luxburg, S Bengio, H Wallach, R Fergus, S Vishwanathan, and R Garnett (Eds.), Vol. 30. Curran Associates, Inc. [https://proceedings.neurips.cc/paper/2017/file/a486cd07e4ac3d270571622f4f316ec5-Paper.pdf](https://proceedings.neurips.cc/paper/2017/file/a486cd07e4ac3d270571622f4f316ec5-Paper.pdf)

<a id="harrison2020">[46]</a> 
Galen Harrison, Julia Hanson, Christine Jacinto, Julio Ramirez, and Blase Ur. 2020. 
An empirical study on the perceived fairness of realistic, imperfect machine learning models. 
In Proceedings of the 2020 Conference on Fairness, Accountability, and Transparency. ACM, New York, NY, USA, 392–402. [https://doi.org/10.1145/3351095.3372831](https://doi.org/10.1145/3351095.3372831)

<a id="srivastava2019">[47]</a> 
Megha Srivastava, Hoda Heidari, and Andreas Krause. 2019. Mathematical Notions vs. 
Human Perception of Fairness. 
In Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining. ACM, New York, NY, USA, 2459–2468. [https://doi.org/10.1145/3292500.3330664](https://doi.org/10.1145/3292500.3330664)

<a id="kearns2018">[48]</a> 
Richard Berk, Hoda Heidari, Shahin Jabbari, Michael Kearns, and Aaron Roth. 2017. 
Fairness in Criminal Justice Risk Assessments: The State of the Art. (3 2017).

<a id="verma2018">[49]</a> 
Sahil Verma and Julia Rubin. 2018. 
Fairness definitions explained. 
In Proceedings of the International Workshop on Software Fairness. ACM, New York, NY, USA,1–7. [https://doi.org/10.1145/3194770.3194776](https://doi.org/10.1145/3194770.3194776)

<a id="hardt2016">[50]</a> 
Moritz Hardt, Eric Price, and Nathan Srebro. 2016. 
Equality of Opportunity in Supervised Learning. 
In Proceedings of the 30th International Conference on Neural Information Processing Systems (NIPS’16). Curran Associates Inc., Red Hook, NY, USA, 3323–3331.

<a id="vanBerkel2021">[51]</a> 
Niels van Berkel, Jorge Goncalves, Daniel Russo, Simo Hosio, and Mikael B. Skov. 2021. 
Effect of Information Presentation on Fairness Perceptions of Machine Learning Predictors. 
In Proceedings of the 2021 CHI Conference on Human Factors in Computing Systems. ACM, New York, NY, USA, 1–13. [https://doi.org/10.1145/3411764.3445365](https://doi.org/10.1145/3411764.3445365)

<a id="berk2017">[52]</a> 
Richard Berk, Hoda Heidari, Shahin Jabbari, Michael Kearns, and Aaron Roth. 2017. 
Fairness in Criminal Justice Risk Assessments: The State of the Art. (3 2017).

<a id="chouldechova2016">[53]</a> 
Alexandra Chouldechova. 2016. 
Fair prediction with disparate impact: A study of bias in recidivism prediction instruments. (10 2016).

<a id="grgichlaca2018">[54]</a> 
Nina Grgic-Hlaca, Muhammad Bilal Zafar, Krishna P Gummadi, and Adrian Weller. 2018. 
Beyond Distributive Fairness in Algorithmic Decision Making: Feature Selection for Procedurally Fair Learning. 
In Proceedings of the AAAI Conference on Artificial Intelligence. Vol. 32.


<a id="kleinberg2016">[55]</a> 
Jon Kleinberg, Sendhil Mullainathan, and Manish Raghavan. 2016. 
Inherent Trade-Offs in the Fair Determination of Risk Scores. (9 2016).

<a id="wang2020">[56]</a> 
Zezhong Wang, Jacob Ritchie, Jingtao Zhou, Fanny Chevalier, and Benjamin Bach. 2021. 
Data Comics for Reporting Controlled User Studies in Human-Computer Interaction.
IEEE Transactionson Visualization and Computer Graphics 27, 2 (2 2021),967–977. [https://doi.org/10.1109/TVCG.2020.3030433](https://doi.org/10.1109/TVCG.2020.3030433)

<a id="saleiro2018">[57]</a> 
Pedro Saleiro, Benedict Kuester, Loren Hinkson, Jesse London, Abby Stevens, Ari Anisfeld, Kit T Rodolfa, and Rayid Ghani. 2018. 
Aequitas: A Bias and Fairness Audit Toolkit.

<a id="dixon2018">[58]</a> 
Lucas Dixon, John Li, Jeffrey Sorensen, Nithum Thain, and Lucy Vasserman. 2018. 
Measuring and Mitigating Unintended Bias in Text Classification.
In Proceedings of the 2018 AAAI/ACM Conference on AI, Ethics, and Society. ACM, New York, NY, USA, 67–73. [https://doi.org/10.1145/3278721.3278729](https://doi.org/10.1145/3278721.3278729)

<a id="bellamy2018">[59]</a> 
R K E Bellamy, K Dey, M Hind, S C Hoffman, S Houde, K Kannan, P Lohia, J Martino, S Mehta, A Mojsilović, S Nagar, K Natesan Ramamurthy, J Richards, D Saha, P Sattigeri, M Singh, K R Varshney, and Y Zhang. 2019. 
AI Fairness 360: An extensible toolkit for detecting and mitigating algorithmic bias. 
IBM Journal of Research and Development 63, 4/5 (2019), 1–4. [https://doi.org/10.1147/JRD.2019.2942287](https://doi.org/10.1147/JRD.2019.2942287)

<a id="stuartgeiger2020">[60]</a> 
R Stuart Geiger, Kevin Yu, Yanlai Yang, Mindy Dai, Jie Qiu, Rebekah Tang, and Jenny Huang. 2020. 
Garbage in, Garbage out? Do Machine Learning Application Papers in Social Computing Report Where Human-Labeled Training Data Comes From?. 
In Proceedings of the 2020 Conference on Fairness, Accountability, and Transparency (FAT* ’20). Association for Computing Machinery, New York, NY, USA, 325–336. [https://doi.org/10.1145/3351095.3372862](https://doi.org/10.1145/3351095.3372862)

<a id="paullada2020">[61]</a> 
Amandalynne Paullada, Inioluwa Deborah Raji, Emily M. Bender, Emily Denton, and Alex Hanna. 2020. 
Data and its (dis)contents: A survey of dataset development and use in machine learning research.(12 2020). [http://arxiv.org/abs/2012.05345](http://arxiv.org/abs/2012.05345)

<a id="gebru2020">[62]</a> 
Timnit Gebru, Google Jamie Morgenstern, Briana Vecchione, and Jennifer Wortman Vaughan. 2020. 
Datasheets for Datasets.

<a id="lee2019">[63]</a> 
Min Kyung Lee, Daniel Kusbit, Anson Kahng, Ji Tae Kim, Xinran Yuan, Allissa Chan, Daniel See, Ritesh Noothigattu, Siheon Lee, Alexandros Psomas, and Ariel D Procaccia. 2019. 
WeBuildAI: Participatory Framework for Algorithmic Governance. 
Proc. ACM Hum.-Comput. Interact. 3, CSCW (11 2019). [https://doi.org/10.1145/3359283](https://doi.org/10.1145/3359283)

<a id="zhouWeb">[64]</a> 
Angela Zhou, David Madras, Inioluwa Raji Raji, Bogdan Kulynych, Smitha Mili, and Richard Zemel. [n. d.]. 
Call for participation: Participatory Approaches to Machine Learning. [https://participatoryml.github.io/](https://participatoryml.github.io/)

<a id="royalsociety2019">[65]</a> 
The Royal Society. 2019. Explainable AI: the basics . 
[https://royalsociety-org.tudelft.idm.oclc.org/-/media/policy/projects/explainable-ai/AI-and-interpretability-policy-briefing.pdf](https://royalsociety-org.tudelft.idm.oclc.org/-/media/policy/projects/explainable-ai/AI-and-interpretability-policy-briefing.pdf)

<a id="bender2018">[66]</a> 
Emily M. Bender and Batya Friedman. 2018. 
Data Statements for Natural Language Processing: Toward Mitigating System Bias and Enabling Better Science.
Transactions of the Association for Computational Linguistics 6 (12 2018). [https://doi.org/10.1162/tacl_a_00041](https://doi.org/10.1162/tacl_a_00041)

<a id="OECD2019">[67]</a> 
OECD. 2019. 
Recommendation of the Council on Artificial Intelligence. 
[https://legalinstruments.oecd.org/en/instruments/OECD-LEGAL-0406](https://legalinstruments.oecd.org/en/instruments/OECD-LEGAL-0406)

<a id="balayn2021Edri">[68]</a> 
Agathe Balayn and Seda Gürses. 2021. 
Beyond Debiasing: Regulating AI and its inequalities. 
[https://edri.org/our-work/if-ai-is-the-problem-is-debiasing-the-solution/](https://edri.org/our-work/if-ai-is-the-problem-is-debiasing-the-solution/)

<a id="kyunglee2017">[69]</a> 
Min Kyung Lee and Su Baykal. 2017. 
Algorithmic Mediation in Group Decisions: Fairness Perceptions of Algorithmically Mediated vs. Discussion-Based Social Division. 
In Proceedings of the 2017 ACM Conference on Computer Supported Cooperative Work and Social Computing (CSCW’17).Association for Computing Machinery, NewYork, NY, USA, 1035–1048. [https://doi.org/10.1145/2998181.2998230](https://doi.org/10.1145/2998181.2998230)

<a id="alfrink2020">[70]</a> 
Kars Alfrink, T. Turel, A. I. Keller, N. Doorn, and G. W. Kortuem. 2020. 
Contestable City Algorithms. 
International Conference on Machine Learning Workshop.

<a id="kalluri2020">[71]</a> 
Pratyusha Kalluri. 2020. 
Don’t ask if artificial intelligence is good or fair, ask how it shifts power. 
Nature 583, 7815 (2020). [https://doi.org/10.1038/d41586-020-02003-2](https://doi.org/10.1038/d41586-020-02003-2)

<a id="lyons2021">[72]</a> 
Henrietta Lyons, Eduardo Velloso, and Tim Miller. 2021. 
Conceptualising Contestability: Perspectives on Contesting Algorithmic Decisions. (2 2021). [https://doi.org/10.1145/3449180](https://doi.org/10.1145/3449180)

<a id="hirsch2017">[73]</a> 
Tad Hirsch, Kritzia Merced, Shrikanth Narayanan, Zac E. Imel, and David C. Atkins. 2017. 
Designing Contestability. 
In Proceedings of the 2017 Conference on Designing Interactive Systems. ACM, New York, NY, USA. [https://doi.org/10.1145/3064663.3064703](https://doi.org/10.1145/3064663.3064703)

<a id="mitra2021">[74]</a> 
Tanushree Mitra. 2021. 
Provocation: Contestability in Large-Scale Interactive {NLP} Systems. 
In Proceedings of the First Workshop on Bridging Human–Computer Interaction and Natural Language Processing. Association for Computational Linguistics, 96–100.

<a id="teliaai2019">[75]</a> 
Telia Company. 2019. 
Guiding Principles on Trusted AI Ethics. 
[https://www.teliacompany.com/globalassets/telia-company/documents/about-telia-company/public-policy/2018/guiding-principles-on-trusted-ai-ethics.pdf](https://www.teliacompany.com/globalassets/telia-company/documents/about-telia-company/public-policy/2018/guiding-principles-on-trusted-ai-ethics.pdf)
















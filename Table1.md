## From values to criteria and their manifestations
| Value       | Criteria  | Manifestations  | 
| ----------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- 
| Privacy     | 1. **Consent for data usage** ([[1]](#GDPR2018), [[2]](#fjeld2020), [[3]](#krafft2020))  <br> 2. **Data protection** ([[2]](#fjeld2020),[[3]](#krafft2020),[[4]](#floridi2019))<br> 3. **Control over data / ability to restrict processing** ([[1]](#GDPR2018), [[2]](#fjeld2020))<br> 4. **Right to rectification** ([[1]](#GDPR2018), [[2]](#fjeld2020), [[3]](#krafft2020)) <br> 5. **Right to erase the data** ([[1]](#GDPR2018), [[2]](#fjeld2020), [[3]](#krafft2020))<br> 6. **Right of access by data subject, data agency** ([[1]](#GDPR2018), [[5]](#IEEE2019)) | - <span style="color:orange">Written declaration of consent</span>([[1]](#GDPR2018)) <br> - <span style="color:orange">Description of what data is collected</span>([[6]](#mehldau2007)) <br> - <span style="color:orange">Description of how data is handled</span> ([[6]](#mehldau2007)) <br> - <span style="color:orange">Purpose statement of data collection</span> ([[6]](#mehldau2007)) <br> - <span style="color:orange">Statement of how long the data is kept</span> ([[6]](#mehldau2007)) <br> - <span style="color:olive">For and submission mechanisms to object data collection and to make complaints</span> ([[7]](#blazevic2021)) <br> - <span style="color:olive">Obfuscation of data</span> ([[3]](#krafft2020))                                                                                                                                                                                                                                   |     |
| Security    | 1. **Resilience to attacks**: protection of privacy ([[8]](#microsoftai2018), [[9]](#hidalgo2021), [[10]](#wachter2019)), vulnerabilities, fallback plans ([[2]](#fjeld2020), [[3]](#krafft2020), [[11]](#morley2020), [[12]](#googleai2018)) <br>2. **Predictability** ([[2]](#fjeld2020), [[3]](#krafft2020), [[13]](#europeancommissionEthicsAI2019)) <br> 3. **Robustness / reliability**: prevent manipulation ([[3]](#krafft2020))                                                                                 | AGAINST INTEGRITY THREATS ([[14]](#xiong2021)): <br> - Training time ([[14]](#xiong2021)). Ex.:<span style="color:olive"><ul><li>Data sanitization ([[15]](#biggio2018), [[16]](#cretu2008))</li><li>Robust learning ([[15]](#biggio2018), [[17]](#globerson2006))</li></ul></span> -    Prediction time ([[14]](#xiong2021)): <span style="color:olive"><ul><li>Model enhancement ([[15]](#biggio2018), [[18]](#lyu2015), [[19]](#goodfellow2014), [[20]](#papernot2016))</li><ul><li>Adversarial learning</li><li>Gradient masking</li><li>Defensive Distillation</li></ul></ul></span> AGAINST PRIVACY THREATS ([[14]](#xiong2021)): <br> - Mitigation techniques ([[21]](#nasr2018)): <span style="color:olive"><ul><li>Restrict prediction vector to top k classes ([[22]](#shokri2017))</li><li>Coarsen the precision of the prediction vector ([[22]](#shokri2017))</li><li>Increase entropy of the prediction vector ([[22]](#shokri2017))</li><li>Use regularization ([[22]](#shokri2017), [[23]](#kaya2020))</li></ul></span>  - Differential privacy mechanisms ([[21]](#nasr2018)):     <span style="color:olive"><ul><li>Differential privacy ([[24]](#ye2021), [[25]](#dwork2006))</li><ul><li>Adversarial regularization ([[21]](#nasr2018))</li><li>MemGuard ([[26]](#jia2019))</li></ul></ul></span> |     |
| Performance | 1. **Correctness of predictions** <br> 2. **Memory efficiency** <br> 3. **Training efficiency <br>** 4. **Energy efficiency** <br> 5. **Data efficiency**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |   - <span style="color:magenta">Accuracy</span> <br> - <span style="color:magenta">False Positive and Negative rates</span> <br> - <span style="color:magenta">False Discovery and Omission rates</span> <br> - <span style="color:magenta">Mean and median error</span> <br> - <span style="color:magenta">R2 score</span> <br> - <span style="color:magenta">Precision and recall rates</span><br> - <span style="color:magenta">Area under ROC curve (AUC)</span> <br> - <span style="color:magenta">Estimation of energy consumption through:</span> <span style="color:black"><ul><li>performance counters</li><li>simulation</li><li>instruction- or architecture-level estimations</li><li>real-time estimation</li></ul></span>- <span style="color:magenta">Estimation of GPU memory consumption</span> <br> - <span style="color:magenta">Wall-clock training time</span>  |
|Respect for public interest | 1. **Desirability of technology** <br> 2. **Benefit to society** <br> 3. **Environmental impact** | - <span style="color:olive">Diverse and inclusive forum for discussion</span> <br> - <span style="color:orange">Measure of social and environmental impact</span> |
Fairness| 1. **Individual fairness** <br> 2. **Demographic parity** <br> 3. **Conditional statistical parity** <br> 4. **Equality of opportunity** <br> 5. **Equalized odds** <br> 6. **Treatment equality** <br> 7. **Test fairness** <br> 8. **Procedural fairness**  | - <span style="color:magenta">Accuracy across groups</span><br> - <span style="color:magenta">False positive and negative rates across groups</span> <br> - <span style="color:magenta">False discovery and omission rates across groups</span><br> - <span style="color:magenta">Pinned AUC</span><br> - <span style="color:olive">Debiasing algorithms</span><br> - <span style="color:olive">Election of protected classes based on user considerations</span> 
| Non-discrimination| 1. **Quality and integrity of data** <br> 2. **Inclusiveness in design** <br> 3. **Accessibility** | - <span style="color:olive">Inclusive data generation process</span> <br> - <span style="color:magenta">Analysis of data for potential biases, data quality assessment</span><br>- <span style="color:olive">Diversity of participant in development process</span><br> - <span style="color:olive">Access to code and technology to all</span>
| Transparency| 1. **Interpretability of data and models** <br> 2. **Enabling human oversight of operations**<br>3. **Accessibility of data and algorithm**<br> 4. **Traceability**<br>5. **Reproducibility** | - <span style="color:orange">Description of data generation process</span><br> - <span style="color:orange">Disclosure of origin and properties of models and data</span><br> - <span style="color:olive">Open access to data and algorithms</span><br> - <span style="color:orange">Notification of usage/interaction</span><br> - <span style="color:orange">Regular reporting</span>
|Explainability| 1. **Ability to understand AI systems and the decision reached**<br> 2. **Traceability** <br> 3. **Enable evaluation** | - <span style="color:olive">Interpretability by design</span><br> - <span style="color:olive">Post-hoc explanations</span>
Contestability | 1. **Enable argumentation / negotiation against a decision** <br> 2. **Citizen empowerment** | - <span style="color:orange">Information of who determines and what constitutes a contestable decision and who is accountable</span><br> - <span style="color:orange">Determination of who can contest the decision (subject or representative)</span><br> - <span style="color:orange">Indication of type of review in place</span><br> - <span style="color:orange">Information regarding the contestability workflow</span><br> - <span style="color:olive">Mechanisms for users to ask questions and record disagreements with system behavior</span>
| Human Control | 1. **User/collective influence** <br> 2. **Human review of automated decision**<br> 3. **Choice of how and whether to delegate** | - <span style="color:olive">Continuous monitoring of system to intervene</span><br> - <span style="color:olive">Establishment levels of human discretion during the use of the system</span><br> - <span style="color:olive">Ability to override the decision made by the system</span>
| Human Agency| 1. **Respect for human autonomy** <br> 2. **Power to decide. Ability to make informed autonomous decision**<br> 3. **Ability to opt out of an automated decision**|- <span style="color:orange">Give knowledge and tools to comprehend and interact with AI system</span><br> - <span style="color:olive">Opportunity to self-assess the system</span>

## References
<a id="GDPR2018">[1]</a> 
European Commission. 2018.
2018 reform of EU data protection rules. 
https://ec.europa.eu/commission/sites/beta-political/files/data-protection-factsheet-changes_en.pdf

<a id="fjeld2020">[2]</a> 
Jessica Fjeld, Nele Achten, Hannah Hilligoss, Adam Nagy, Madhulika Srikumar. 2020.
Principled Artificial Intelligence: Mapping Consensus in Ethical and Rights-Based Approaches to Principles for AI. 
SSRN Electronic Journal (2020) https://doi.org/10.2139/ssrn.3518482

<a id="krafft2020">[3]</a> 
AI Ethics Impact Group (AIEIG). 2020. 
From Principles to Practice An interdisciplinary framework to operationalise AI ethics. 
https://www.ai-ethics-impact.org/resource/blob/1961130/c6db9894ee73aefa489d6249f5ee2b9f/aieig---report---download-hb-data.pdf

<a id="floridi2019">[4]</a> 
Luciano Floridi. 2019. 
Translating Principles into Practices of Digital Ethics: Five Risks of Being Unethical. 
Philosophy & Technology 32, 2 (6 2019). https://doi.org/10.1007/s13347-019-00354-x

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
SSRN Electronic Journal (2021). https://doi.org/10.2139/ssrn.3776353

<a id="microsoftai2018">[8]</a> 
Microsoft. 2018. 
AI Principles.
https://www.microsoft.com/en-us/ai/responsible-ai?activetab=pivot1%3aprimaryr6

<a id="hidalgo2021">[9]</a> 
César Hidalgo, Diana Orghian, Jordi Albo-Canals, Filipa de Almeida, and Natalia Martin. 2021. 
How Humans Judge Machines. 
MIT Press. https://hal.archives- ouvertes.fr/hal-03058652

<a id="wachter2019">[10]</a> 
Sandra Wachter and Brent Mittelstadt. 2019. 
Right to Reasonable Inferences: Re-Thinking Data Protection Law in the Age of Big Data and AI. 
Columbia Business Law Review 2 (2019), 494–620.

<a id="morley2020">[11]</a> 
Jessica Morley, Luciano Floridi, Libby Kinsey, and Anat Elhalal. 2020. 
From What to How: An Initial Review of Publicly Available AI Ethics Tools, Methods and Research to Translate Principles into Practices. 
Science and Engineering Ethics 26 (2020), 2141–2168. https://doi.org/10.1007/s11948-019-00165-5

<a id="googleai2018">[12]</a> 
Google. 2018. 
AI at Google: Our Principles. 
https://www.blog.google/technology/ai/ai-principles/

<a id="europeancommissionEthicsAI2019">[13]</a> 
European Commission. 2019. 
Ethics guidelines for trustworthy AI. 
https://www.aepd.es/sites/default/files/2019-12/ai-ethics-guidelines.pdf

<a id="xiong2021">[14]</a> 
Pulei Xiong, Scott Buffett, Shahrear Iqbal, Philippe Lamontagne, Mohammad Mamun, and Heather Molyneaux. 2021. 
Towards a Robust and Trustworthy Machine Learning System Development. (1 2021).

<a id="biggio2018">[15]</a> 
Battista Biggio and Fabio Roli. 2018. 
Wild patterns: Ten years after the rise of adversarial machine learning. 
Pattern Recognition 84 (12 2018), 317–331. https://doi.org/10.1016/j.patcog.2018.07.023

<a id="cretu2008">[16]</a> 
Gabriela F. Cretu, Angelos Stavrou, Michael E. Locasto, Salvatore J. Stolfo, and Angelos D. Keromytis. 2008. 
Casting out Demons: Sanitizing Training Data for Anomaly Sensors.
In 2008 IEEE Symposiumon Security and Privacy (sp2008).IEEE,81–95. https://doi.org/10.1109/SP.2008.11

<a id="globerson2006">[17]</a> 
Amir Globerson and Sam Roweis. 2006. 
Nightmare at test time. 
In Proceedings of the 23rd international conference on Machine learning - ICML ’06. ACMPress, New York, NewYork, USA, 353–360. https://doi.org/10.1145/1143844.1143889

<a id="lyu2015">[18]</a> 
Chunchuan Lyu, Kaizhu Huang, and Hai-Ning Liang. 2015. 
A Unified Gradient Regularization Family for Adversarial Examples. 
In 2015 IEEE International Conference on Data Mining.IEEE,301–309. https://doi.org/10.1109/ICDM.2015.84

<a id="goodfellow2014">[19]</a> 
Ian J. Goodfellow, Jonathon Shlens, and Christian Szegedy. 2014. 
Explaining and Harnessing Adversarial Examples. (12 2014).

<a id="papernot2016">[20]</a> 
Nicolas Papernot, Patrick McDaniel, Xi Wu, Somesh Jha, and Ananthram Swami. 2016. 
Distillation as a Defense to Adversarial Perturbations Against Deep Neural Networks. 
In 2016 IEEE Symposium on Security and Privacy (SP). IEEE, 582–597. https://doi.org/10.1109/SP.2016.41

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
https://doi.org/10.1007/11681878_14

<a id="jia2019">[25]</a> 
Jinyuan Jia, Ahmed Salem, Michael Backes, Yang Zhang, and Neil Zhenqiang Gong. 2019. 
MemGuard: Defending against Black-Box Membership Inference Attacks via Adversarial Examples. (9 2019).


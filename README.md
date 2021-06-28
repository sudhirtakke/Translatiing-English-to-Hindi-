# Translatiing-English-to-Hindi-
Seq2Seq Model with Attention Mechanism for translating English to Hindi

The **encoder-decoder** model for recurrent neural networks is an architecture for **sequence-to-sequence** prediction problems.

It is comprised of **two sub-models**, as its name suggests:

  - **Encoder**: The *encoder* is responsible for *stepping through* the *input time steps* and *encoding* the *entire sequence into a fixed length vector* called a **context vector**.
<br><br>
  - **Decoder**: The *decoder* is responsible for *stepping through* the *output time steps while reading from* the **context vector**.

A **problem** with the *architecture* is that **performance** is **poor** on *long input or output sequences*. 

- The **reason** is believed to be because of the **fixed-sized internal representation** used by the *encoder*.<br>

 
**Attention** is an extension to the architecture that **addresses** this **limitation**. 

 - It **works** by first *providing* a *richer context from* the *encoder to* the *decoder*. 
 
 
 - And a **learning mechanism** where the *decoder can learn where to pay* **attention** in the *richer encoding when predicting each time step in* the *output sequence*.

<br> 
<center><img src="https://raw.githubusercontent.com/insaid2018/DeepLearning/master/images/attention_mechanism.png"/></center
 
 **Here are few examples of translation using the model.**
  
 translate('hello')<br>
 Input: <start> hello <end> <br>
 Predicted translation: नमसकार। <end> <br>
  
 translate('How are you?')<br>
 Input: <start> how are you ? <end> <br>
 Predicted translation: आप कस ह ? <end> <br>
  
  
 translate('he is a good person')<br>
 Input: <start> he is a good person <end> <br>
 Predicted translation: वह अचछा इनसान ह। <end> <br>

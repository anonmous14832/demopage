## ZenFlow: Zero-Shot Generative Speech Synthesis via Alignment-based Speech Representation Learning


### Abstract

In this paper we propose ZenFlow: a framework for Zero-Shot Generative Speech Synthesis via Alignment-based Speech Representation Learning. ZenFlow uses an alignment-based mechanism to learn a vector quantized phoneme representation that generalizes well to unseen data and is robust to data degradation, without sacrificing pronunciation. Departing from existing representation learning strategies in speech, we propose a factorized speech representation that provides large scale training without text-labelled data and supports independent and fine-grained control in speech synthesis downstream tasks. We leverage this factorized representation to develop ZenTTS: a non-autoregressive speech synthesis framework that performs well on zero-shot and transfer tasks. Our evaluation shows that our ZenFlow representation is able to factorize speech into controllable and interpretable factors, while preserving audio fidelity. Human Evaluation on downstream tasks show that ZenTTS is comparable to recent state-of-the-art zero-shot TTS models in terms of naturalness and speaker similarity.

### Robustness to Degradation (Section 3.3)
<table>
   <thead>
      <tr>
         <th style="text-align: center">Degraded</th>
         <th style="text-align: center">EnCodec 6.0kbps</th>
         <th style="text-align: center">EnCodec 1.5kbps</th>
         <th style="text-align: center">ZenFlow-Continuous 0.947 kbps + F0, Energy </th>
         <th style="text-align: center">ZenFlow-Discrete 2.153 kbps </th>
      </tr>
   </thead>
   Degradation 8khz
   <tbody>
      <tr>      
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/61-70968-0016_deg.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/encodec_6p0bw-61-70968-0016_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/encodec_1p5bw-61-70968-0016_hat.wav" type="audio/wav"></audio></td>   
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/zenflow-continuous-61-70968-0016_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/zenflow-discrete-61-70968-0016_hat.wav" type="audio/wav"></audio></td>
      </tr>
      <tr>      
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/121-121726-0010_deg.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/encodec_6p0bw-121-121726-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/encodec_1p5bw-121-121726-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/zenflow-continuous-121-121726-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/zenflow-discrete-121-121726-0010_hat.wav" type="audio/wav"></audio></td>
      </tr>
      <tr>      
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/237-134500-0010_deg.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/encodec_6p0bw-237-134500-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/encodec_1p5bw-237-134500-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/zenflow-continuous-237-134500-0010_hat.wav" type="audio/wav"></audio></td>      
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/8khz/zenflow-discrete-237-134500-0010_hat.wav" type="audio/wav"></audio></td>         
      </tr>            
   </tbody>
</table>   

<table>
   <thead>
      <tr>
         <th style="text-align: center">Degraded</th>
         <th style="text-align: center">EnCodec 6.0kbps</th>
         <th style="text-align: center">EnCodec 1.5kbps</th>
         <th style="text-align: center">ZenFlow-Continuous 0.947 kbps + F0, Energy </th>
         <th style="text-align: center">ZenFlow-Discrete 2.153 kbps </th>
      </tr>
   </thead>
   Degradation 16khz
   <tbody>
      <tr>      
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/61-70968-0016_deg.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/encodec_6p0bw-61-70968-0016_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/encodec_1p5bw-61-70968-0016_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/zenflow-continuous-70968-0016_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/zenflow-discrete-61-70968-0016_hat.wav" type="audio/wav"></audio></td>      
      </tr>
      <tr>      
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/121-121726-0010_deg.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/encodec_6p0bw-121-121726-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/encodec_1p5bw-121-121726-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/zenflow-continuous-121-121726-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/zenflow-discrete-121-121726-0010_hat.wav" type="audio/wav"></audio></td>      
      </tr>
      <tr>      
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/237-134500-0010_deg.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/encodec_6p0bw-237-134500-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/encodec_1p5bw-237-134500-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/zenflow-continuous-237-134500-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/16khz/zenflow-discrete-237-134500-0010_hat.wav" type="audio/wav"></audio></td>      
      </tr>            
   </tbody>
</table>   

<table>
   <thead>
      <tr>
         <th style="text-align: center">Degraded</th>
         <th style="text-align: center">EnCodec 6.0kbps</th>
         <th style="text-align: center">EnCodec 1.5kbps</th>
         <th style="text-align: center">ZenFlow-Continuous 0.947 kbps + F0, Energy </th>
         <th style="text-align: center">ZenFlow-Discrete 2.153 kbps </th>
      </tr>
   </thead>
   Resynthesis 22khz
   <tbody>
      <tr>      
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/61-70968-0016_deg.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/encodec_6p0bw-61-70968-0016_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/encodec_1p5bw-61-70968-0016_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/zenflow-continuous-61-70968-0016_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/zenflow-discrete-61-70968-0016_hat.wav" type="audio/wav"></audio></td>      
      </tr>
      <tr>      
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/121-121726-0010_deg.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/encodec_6p0bw-121-121726-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/encodec_1p5bw-121-121726-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/zenflow-continuous-121-121726-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/zenflow-discrete-121-121726-0010_hat.wav" type="audio/wav"></audio></td>      
      </tr>
      <tr>      
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/237-134500-0010_deg.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/encodec_6p0bw-237-134500-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/encodec_1p5bw-237-134500-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/zenflow-continuous-237-134500-0010_hat.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/robustness/22khz/zenflow-discrete-237-134500-0010_hat.wav" type="audio/wav"></audio></td>      
      </tr>            
   </tbody>   
</table>    
      

### Zero-shot TTS (Section 4.2)
<table>
   <thead>
      <tr>
         <th style="text-align: center">Text</th>
         <th style="text-align: center">Ground Truth</th>
         <th style="text-align: center">Reference</th>
         <th style="text-align: center">ZenFlow-MIX </th>
         <th style="text-align: center">Vall-E</th>
      </tr>
   </thead>
   <tbody>
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">They moved thereafter cautiously about the hut, groping before and about them to find something to show that Warrenton had fulfilled his mission.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-gt/0_61-70970-0024_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-reference/0_prompt-61-70970-0027.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-zenflowtts-mixed-libritts30k-librivox20x/0_61-70970-0024_1.0_hat_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-vall-e/0_valle_61-70970-0024_normalized.wav" type="audio/wav"></audio></td>
      </tr>
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">And lay me down in thy cold bed, and leave my shining lot.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-gt/1_908-157963-0027_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-reference/1_prompt-908-157963-0011.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-zenflowtts-mixed-libritts30k-librivox20x/1_908-157963-0027_1.0_hat_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-vall-e/1_valle_908-157963-0027_normalized.wav" type="audio/wav"></audio></td>         
      </tr>
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">Number ten, fresh nelly is waiting on you. -Good night husband!</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-gt/2_1089-134686-0004_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-reference/2_prompt-1089-134691-0001.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-zenflowtts-mixed-libritts30k-librivox20x/2_1089-134686-0004_1.0_hat_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-vall-e/2_valle_1089-134686-0004_normalized.wav" type="audio/wav"></audio></td>      
      </tr>
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">Yea, his honourable worship is within. But he hath a godly minister or two with him, and likewise a leech.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-gt/3_1221-135767-0014_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-reference/3_prompt-1221-135767-0012.wav" type="audio/wav"></audio></td>         
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-zenflowtts-mixed-libritts30k-librivox20x/3_1221-135767-0014_1.0_hat_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-vall-e/3_valle_1221-135767-0014_normalized.wav" type="audio/wav"></audio></td>
      </tr>
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">Instead of shoes, the old man wore boots with turnover tops, and his blue coat had wide cuffs of gold braid.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-gt/4_1284-1180-0002_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-reference/4_prompt-1284-1181-0016.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-zenflowtts-mixed-libritts30k-librivox20x/4_1284-1180-0002_1.0_hat_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-vall-e/4_valle_1284-1180-0002_normalized.wav" type="audio/wav"></audio></td>
      </tr>
      <tr>
         <td style="text-align: left;vertical-align:middle;width: 420px;">The army found the people in poverty and left them in comparative wealth.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-gt/5_4077-13754-0000_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-reference/5_prompt-4077-13751-0008.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-zenflowtts-mixed-libritts30k-librivox20x/5_4077-13754-0000_1.0_hat_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-vall-e/5_valle_4077-13754-0000_normalized.wav" type="audio/wav"></audio></td>
      </tr>
      <tr>
         <td style="text-align: left;vertical-align:middle;width: 420px;">Thus did this humane and right-minded father comfort his unhappy daughter; and her mother, embracing her again, did all she could to soothe her feelings.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-gt/6_5639-40744-0020_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-reference/6_prompt-5639-40744-0023.wav" type="audio/wav"></audio></td>         
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-zenflowtts-mixed-libritts30k-librivox20x/6_5639-40744-0020_1.0_hat_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-vall-e/6_valle_5639-40744-0020_normalized.wav" type="audio/wav"></audio></td>         
      </tr>
      <tr>
         <td style="text-align: left;vertical-align:middle;width: 420px;">He was in deep converse with the clerk, and entered the hall holding him by the arm.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-gt/7_61-70970-0007_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-reference/7_prompt-61-70970-0018.wav" type="audio/wav"></audio></td>         
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-zenflowtts-mixed-libritts30k-librivox20x/7_61-70970-0007_1.0_hat_normalized.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/zeroshot/pps-vall-e/7_valle_61-70970-0007_normalized.wav" type="audio/wav"></audio></td>
      </tr>
   </tbody>
</table>


### Zero-shot TTS with Language Transfer (Section 4.3) (Updated on paper)
#### LJS (English speaker speaks English with English and German accent): 
Reference  
<audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/timbre_speaker_en-us-female-LJ022-0023.wav" type="audio/wav"></audio>
<table>
   <thead>
      <tr>
      <th style="text-align: center">Text</th>
         <th style="text-align: center">Ground Truth Phonemes</th>
         <th style="text-align: center">ZenTTS with English ZenFlow (English accent)</th>
         <th style="text-align: center">ZenTTS with English ZenFlow (German accent)</th>
         <th style="text-align: center">ZenTTS with Multilingual ZenFlow (English accent)</th>
         <th style="text-align: center">ZenTTS with Multilingual ZenFlow (German accent)</th>
      </tr>
   </thead>
   <tbody>
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">He was in consequence put out of the protection of their internal law, end quote. Their code was a subject of some curiosity.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ground_truth/LJ003-0111.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/en_US/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ003-0111.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/en_DE/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ003-0111.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/en_US/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ003-0111.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/en_DE/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ003-0111.wav" type="audio/wav"></audio></td>
      </tr>
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">The original plan called for the President to spend only one day in the State, making whirlwind visits to Dallas, Fort Worth, San Antonio, and Houston.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ground_truth/LJ029-0022.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/en_US/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ029-0022.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/en_DE/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ029-0022.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/en_US/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ029-0022.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/en_DE/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ029-0022.wav" type="audio/wav"></audio></td>
      </tr>
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">and others who were present say that no agent was inebriated or acted improperly.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ground_truth/LJ048-0228.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/en_US/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ048-0228.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/en_DE/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ048-0228.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/en_US/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ048-0228.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/en_DE/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ048-0228.wav" type="audio/wav"></audio></td>
      </tr>
   </tbody>
</table>

#### LJS (English speaker speaks German with English and German accent): 
Reference    
<audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/timbre_speaker_en-us-female-LJ022-0023.wav" type="audio/wav"></audio>
<table>
   <thead>
      <tr>
      <th style="text-align: center">Text</th>
         <th style="text-align: center">Ground Truth Phonemes</th>
         <th style="text-align: center">ZenTTS with English ZenFlow (German Accent)</th>
         <th style="text-align: center">ZenTTS with English ZenFlow (English accent)</th>
         <th style="text-align: center">ZenTTS with Multilingual ZenFlow (German accent)</th>
         <th style="text-align: center">ZenTTS with Multilingual ZenFlow (English accent)</th>   
      </tr>
   </thead>
   <tbody>
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">Und nun geschah das große Unglück, daß dieser so eindeutige elementare Aufruhr so gründlich fehlgedeutet wurde.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ground_truth/saemtliche_schriften4_43_F000048.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/de_DE/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/saemtliche_schriften4_43_F000048.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/de_US/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/saemtliche_schriften4_43_F000048.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/de_DE/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/saemtliche_schriften4_43_F000048.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/de_US/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/saemtliche_schriften4_43_F000048.wav" type="audio/wav"></audio></td>   
      </tr>   
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">Der Vezier nahm alles, was ihm der König gab, durchwanderte die Wüste in der Länge und in der Breite, bis er in das Land des Königs Schamech kam.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ground_truth/tausend_und_eine_nacht_band_2_08_F000069.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/de_DE/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/tausend_und_eine_nacht_band_2_08_F000069.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/de_US/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/tausend_und_eine_nacht_band_2_08_F000069.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/de_DE/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/tausend_und_eine_nacht_band_2_08_F000069.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/de_US/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/tausend_und_eine_nacht_band_2_08_F000069.wav" type="audio/wav"></audio></td>
      </tr>
     <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">die Kirche verließen, brauste die Orgel Triumph und die Glocke</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ground_truth/totenhochzeit_03_F000112.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/de_DE/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/totenhochzeit_03_F000112.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/de_US/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/totenhochzeit_03_F000112.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/de_DE/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/totenhochzeit_03_F000112.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ljs/de_US/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/totenhochzeit_03_F000112.wav" type="audio/wav"></audio></td>
      </tr>
   </tbody>
</table>

#### Arnold (German speaker speaks English with English and German accent)
Reference  
<audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/timbre_speaker_arnold_reference_mono.wav" type="audio/wav"></audio>
<table>
   <thead>
      <tr>
      <th style="text-align: center">Text</th>
         <th style="text-align: center">Ground Truth Phonemes</th>
         <th style="text-align: center">ZenTTS with English ZenFlow (English Accent)</th>
         <th style="text-align: center">ZenTTS with English ZenFlow (German accent)</th>
         <th style="text-align: center">ZenTTS with Multilingual ZenFlow (English accent)</th>
         <th style="text-align: center">ZenTTS with Multilingual ZenFlow (German accent)</th>   
      </tr>
   </thead>
   <tbody>
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">He was in consequence put out of the protection of their internal law, end quote. Their code was a subject of some curiosity.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ground_truth/LJ003-0111.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/en_US/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ003-0111.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/en_DE/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ003-0111.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/en_US/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ003-0111.wav" type="audio/wav"></audio></td>   
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/en_DE/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ003-0111.wav" type="audio/wav"></audio></td>
      </tr>
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">The original plan called for the President to spend only one day in the State, making whirlwind visits to Dallas, Fort Worth, San Antonio, and Houston.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ground_truth/LJ029-0022.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/en_US/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ029-0022.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/en_DE/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ029-0022.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/en_US/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ029-0022.wav" type="audio/wav"></audio></td>            
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/en_DE/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ029-0022.wav" type="audio/wav"></audio></td>
      </tr>
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">and others who were present say that no agent was inebriated or acted improperly.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ground_truth/LJ048-0228.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/en_US/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ048-0228.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/en_DE/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ048-0228.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/en_US/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ048-0228.wav" type="audio/wav"></audio></td>            
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/en_DE/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/LJ048-0228.wav" type="audio/wav"></audio></td>
      </tr>
   </tbody>
</table>

#### Arnold (German speaker speaks German with German and English accent)
Reference. 
<audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/timbre_speaker_arnold_reference_mono.wav" type="audio/wav"></audio>
<table>
   <thead>
      <tr>
      <th style="text-align: center">Text</th>
         <th style="text-align: center">Ground Truth Phonemes</th>
         <th style="text-align: center">ZenTTS with English ZenFlow (German Accent)</th>
         <th style="text-align: center">ZenTTS with English ZenFlow (English accent)</th>
         <th style="text-align: center">ZenTTS with Multilingual ZenFlow (German accent)</th>
         <th style="text-align: center">ZenTTS with Multilingual ZenFlow (English accent)</th>
      </tr>
   </thead>
   <tbody>
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">Und nun geschah das große Unglück, daß dieser so eindeutige elementare Aufruhr so gründlich fehlgedeutet wurde.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ground_truth/saemtliche_schriften4_43_F000048.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/de_DE/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/saemtliche_schriften4_43_F000048.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/de_US/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/saemtliche_schriften4_43_F000048.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/de_DE/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/saemtliche_schriften4_43_F000048.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/de_US/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/saemtliche_schriften4_43_F000048.wav" type="audio/wav"></audio></td>
      </tr>   
      <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">Der Vezier nahm alles, was ihm der König gab, durchwanderte die Wüste in der Länge und in der Breite, bis er in das Land des Königs Schamech kam.</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ground_truth/tausend_und_eine_nacht_band_2_08_F000069.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/de_DE/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/tausend_und_eine_nacht_band_2_08_F000069.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/de_US/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/tausend_und_eine_nacht_band_2_08_F000069.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/de_DE/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/tausend_und_eine_nacht_band_2_08_F000069.wav" type="audio/wav"></audio></td>            
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/de_US/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/tausend_und_eine_nacht_band_2_08_F000069.wav" type="audio/wav"></audio></td>
      </tr>
     <tr>
      <td style="text-align: left;vertical-align:middle;width: 420px;">die Kirche verließen, brauste die Orgel Triumph und die Glocke</td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/ground_truth/totenhochzeit_03_F000112.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/de_DE/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/totenhochzeit_03_F000112.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/de_US/zenflowtts-spkenctrsnf-alldata-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/totenhochzeit_03_F000112.wav" type="audio/wav"></audio></td>
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/de_DE/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/totenhochzeit_03_F000112.wav" type="audio/wav"></audio></td>            
         <td style="text-align: center"><audio controls style="width: 150px;"><source src="wavs/multilingual/arnolds/de_US/zenflowtts-spkenctrsnf-alldata-backboneall-F0transf-pdropdur0p0F0out0p0-2048ntokens-lngemb/totenhochzeit_03_F000112.wav" type="audio/wav"></audio></td>
      </tr>
   </tbody>
</table>

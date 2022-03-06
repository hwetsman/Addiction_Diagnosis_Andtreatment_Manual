```mermaid
flowchart TB

regularly_using(Note what the patient <br>is regularly using in the <br>last few months)
can_identify{Can patient identify <br>pre-drug symptoms?}
   regularly_using--->can_identify
what_kind{What kind?}
   can_identify--->|Yes|what_kind
   trauma{Did patient have <br>serious sustained <br>pre-drug trauma?}
      what_kind--->|Increased DA|trauma
      consider_low(Consider low dopamine <br>genetics hidden by <br>pre-drug trauma)
         trauma--->|Yes|consider_low
      what_drug(What drug was <br>used first for <br>symtpoms of increased <br>dopamine?)
         trauma--->|No|what_drug
         how_long(How long before <br>they started using <br>stimulants?)
            what_drug--->how_long
            low_now{Evidence of decreased <br>dopamine now?}
               how_long--->low_now
               gaba(Consider decreased <br>GABA tone)
                  low_now--->|No|gaba
                  really(Consider if <br>it's really <br>addiction)
                     gaba--->really
   first_drug(What was their <br>first drug <br>and what <br>behavior did <br>they use <br>before it?)
      what_kind--->|Decreased DA|first_drug
      works_now(What drug <br>works best <br>now?)
         first_drug--->works_now
         side_effects(Which do they <br>use for symptoms <br>and which for <br>side effects or <br>oblivion?)
            works_now--->side_effects
favorite(What is favorite <br>drug for peak <br>effect even <br>if transitory?)
   can_identify--->|No|favorite
   what_does(What does it do that others don't?)
      favorite--->what_does
      low_da{Low dopamine symptoms now?}
         what_does--->low_da
         op_vs_da{Opioid vs dopamine receptor}
            low_da--->op_vs_da
            side_effects--->op_vs_da
            low_now--->|Yes|op_vs_da
               low_gaba(Consider decreased GABA tone)
                  low_da--->|No|low_gaba
            da(Titrate long acting bupropion or other to increase dopamine tone)
               op_vs_da--->|Dopamine|da
            op(Titrate buprenorphine)
               op_vs_da--->|Opioid|op
               still_smoking{Is patient still smoking?}
                  op--->still_smoking
                  da--->still_smoking
                  cues{Continued smoking due to stereotypical cues?}
                     still_smoking--->|Yes|cues
                     campral(Consider acamprosate)
                        cues--->|Yes|campral
                     raise_gaba(Consider raising dose or GABAb)
                        still_smoking--->|No|raise_gaba
                        cues--->|No|raise_gaba
                        other(Evaluate for adverse effects, residual symptoms and co-occurring disorders)
                           raise_gaba--->other
                           campral--->other


```

@author=Squandor
@title=Wunderground
@version=0.0.8
@description=Small plugin which uses the weatherground.com api. you just need an api key and set this in 'general_settings: wunderground:'

@summary=To use the weather underground plugin you need to have the api set in the general_settings under server.
<pre>
general_settings:
  wunderground:
    - api = 123456
    - language = en
</pre>
Next you need the following settings on an component:
<pre>
wunderground:
  display_components:
    components:
      - wunderground[forecast]
      - wunderground[condition]
  wunderground:
    forecast:
      location: Nijmegen, NL
    condition:
      location: Breda, NL
</pre>
With the title forecast you will get an forecast template, with the condition template you will get an weather widget of today.

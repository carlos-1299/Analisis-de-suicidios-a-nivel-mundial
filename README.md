# Analisis-de-suicidios a nivel mundial y nacional
<img src="banner_mundial.jpeg" style="width:100%;">
 Enlace del video:
*https://youtu.be/BZ65P8OL3Dg
import io
import base64
from IPython.display import HTML

video = io.open('inteligencia.mp4', 'r+b').read()
encoded = base64.b64encode(video)
HTML(data='''<video alt="test" controls>
                <source src="data:video/mp4;base64,{0}" type="video/mp4" />
             </video>'''.format(encoded.decode('ascii')))

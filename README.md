Language translation stands out as one of the most intricate human tasks for machines to master, yet it holds immense potential to unite the world as one global community. With our project, we aim to contribute to the evolution of machine translation, moving toward a future where technology seamlessly bridges language barriers. 

Our goal is to integrate the current state-of-the-art into a single, user-friendly product that evolves continuously, remaining open to harnessing the latest advancements in machine intelligence, including deep learning. To realize our vision, we seek to develop superior machine translation technology that can extract deeper insights from data, adapt to various contexts, and offer easy deployment options. 

# Lingvanex
Lingvanex is a cutting-edge technology company specializing in advanced language solutions, primarily focusing on machine translation and speech recognition. Their products are designed to enhance communication and streamline processes across various industries. Here’s a brief overview of their main offerings.

# Key Products
* Machine Translation: Lingvanex provides robust machine translation services that support over 100 languages. Their solutions can be deployed on-premise, via SDK, or through cloud integration, making it versatile for different business needs. The technology ensures high-quality translations for large volumes of text, documents, and websites, all while maintaining data privacy and security.

* Speech Recognition: The company offers a self-hosted speech recognition software that operates in 93 languages. This solution allows organizations to process and analyze speech locally, ensuring full privacy protection and unlimited usage. It is particularly beneficial for businesses that require accurate voice recognition without relying on internet connectivity.


# Your first translation with Lingvanex

Discover the Power of Lingvanex Translator Service

Unlock the potential of your applications with Lingvanex Translator, a cutting-edge cloud-based neural machine translation service. Compatible with any operating system, free translation api Python Lingvanex enables the creation of intelligent, multi-lingual solutions for all supported languages. Whether you are looking for a python translation API, or need to translate text efficiently, Lingvanex offers a powerful solution for developers.

With Lingvanex, you can effortlessly translate both text and HTML pages, enhancing your global reach and communication capabilities. Our free translation API for Python allows you to start integrating translation functionality into your projects quickly and easily. Additionally, our python library for translation ensures smooth integration with minimal setup. You can also explore a specialized python language translation library, making it easy to build language tools.

Explore the capabilities of the [Lingvanex Cloud API](https://lingvanex.com/en/translationapi/) and learn more about our [Secure On-Premise Machine Translation](https://lingvanex.com/). This versatile tool provides developers with a **python library to translate text**, offering a robust way to handle translations in your application. For those seeking a free python translation API, Lingvanex offers solutions that meet all levels of demand.

# Installation
You can install the library with PyPI using pip:

```
pip install lingvanex
```

# Requirements
* Python version >= 3.6
* Requests module version >= 2.0


# Getting the list of languages
To retrieve the list of languages, perform a GET request with the authentication key as follows:
```
import requests

url = "https://api-b2b.backenster.com/b1/api/v3/getLanguages?platform=api&code=en_GB"

headers = {"accept": "application/json"}

response = requests.get(url, headers=headers)

print(response.text)
```

Options:
* `url`: https://api-b2b.backenster.com/b1/api/v3/getLanguages
* `platform`: api
* `Authorization`: The key must be obtained in advance
* `code`: the language code in the format “language code_code of the country”, which is used to display the names of the languages. The language code is represented only in lowercase letters, the country code only in uppercase letters (example en_GB, es_ES, ru_RU etc). If this option is not present, then English is used by default.


# Translate Python Text
This POST method translates text and HTML single string or arrays with the authentication key. Also it performs transliteration, language auto detection.

```
import requests

url = "https://api-b2b.backenster.com/b1/api/v3/translate"

payload = {
    "platform": "api",
    "from": "en_GB",
    "to": "de_DE",
    "data": "Some text",
    "translateMode": "html",
    "enableTransliteration": True
}
headers = {
    "accept": "application/json",
    "content-type": "application/json"
}

response = requests.post(url, json=payload, headers=headers)

print(response.text)
```

Options:
* `url`: https://api-b2b.backenster.com/b1/api/v3/translate
* `platform`: api
* `Authorization`: The key must be obtained in advance
* `from`: the language code in the format “language code_code of the country” from which the text is translated. The language code is represented only in lowercase letters, the country code only in uppercase letters (example en_GB, es_ES, ru_RU and etc.). If this parameter is not present, the auto-detect language mode is enabled.
* `to`: language code in the format “language code_code of the country” to which the text is translated (required)
* `data`: data for translation.
* `translateMode`: Describe the input text format. Possible value is "html" for translating and preserving html structure. If the value is not specified or is other than "html" then plain text is translating.
* `enableTransliteration`: If true response includes sourceTransliteration and targetTransliteration fields.

# Why Choose Lingvanex?
﻿With seven years of experience, Lingvanex prioritizes quality and innovation. Here are some of the key features that define our company:
 
* Consistent Technical Support. Our group of specialists are available to assist you with any problems or questions you may have. This ensures that your translation requests are handled efficiently, saving you time and effort.

* Ongoing Model Training. Lingvanex is committed to continuous improvement. We frequently update and improve our translation models using the latest technology. This constant development results in more accurate translations.

* Skilled Professionals. Our linguists aren't only multilingual, but also have specialized cultural knowledge. This knowledge ensures that technical terms, nuances and cultural context are reflected in our translations.

* Feedback system. We actively collect feedback from our users, which plays a crucial role in improving our services. With this, we can make changes when training models that will meet their needs and preferences.

* Advanced machine learning technology. Using advanced machine learning algorithms and an extensive database allows us to make our translations accurate not only linguistically, but also context-aware. 


# Issues
If you are having problems using the library, please [contact](https://lingvanex.com/en/contact-us/) us.

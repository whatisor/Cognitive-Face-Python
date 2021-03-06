Ubuntu 14.04:

sudo apt-get install python-pip

pip install cognitive_face

```

Use it:

```python
import cognitive_face as CF

KEY = 'subscription key'  # Replace with a valid Subscription Key here.
CF.Key.set(KEY)

BASE_URL = 'https://westus.api.cognitive.microsoft.com/face/v1.0/'  # Replace with your regional Base URL
CF.BaseUrl.set(BASE_URL)

img_url = 'https://raw.githubusercontent.com/Microsoft/Cognitive-Face-Windows/master/Data/detection1.jpg'
result = CF.face.detect(img_url)
print result
```

## Running the sample

A sample desktop application is also provided.

To run it, install the following prerequisites:

- [Python 2.7](https://www.python.org/downloads/) (version 3 is **not** currently supported, you can vote for this feature [here](https://github.com/Microsoft/Cognitive-Face-Python/issues/30))
- [wxPython 3.0.2](https://sourceforge.net/projects/wxpython/files/wxPython/3.0.2.0/) (version 4 is **not** currently supported)

Then run the following:

Install wxpython3.0:

Down load source here

https://sourceforge.net/projects/wxpython/files/wxPython/3.0.2.0/wxPython-src-3.0.2.0.tar.bz2/download

sudo apt-get install gtk+-2.0

Extract wxPython-src-3.0.2.0.tar.bz2 and build by

./configure

make

sudo make install

```bash
git clone https://github.com/Microsoft/Cognitive-Face-Python.git
cd Cognitive-Face-Python
pip install -r requirements.txt
python sample
```

![Sample app](./Assets/sample_screenshot.png)


## Contributing

We welcome contributions. Feel free to file issues and pull requests on the repo and we'll address them as we can. Learn more about how you can help on our [Contribution Rules & Guidelines](</CONTRIBUTING.md>).

You can reach out to us anytime with questions and suggestions using our communities below:
 - **Support questions:** [StackOverflow](<https://stackoverflow.com/questions/tagged/microsoft-cognitive>)
 - **Feedback & feature requests:** [Cognitive Services UserVoice Forum](<https://cognitive.uservoice.com>)

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Updates
* [Face API Release Notes](https://docs.microsoft.com/en-us/azure/cognitive-services/face/releasenotes)

## License
All Microsoft Cognitive Services SDKs and samples are licensed with the MIT License. For more details, see
[LICENSE](</LICENSE.md>).

Sample images are licensed separately, please refer to [LICENSE-IMAGE](</LICENSE-IMAGE.md>)

## Developer Code of Conduct
Developers using Cognitive Services, including this sample, are expected to follow the “Developer Code of Conduct for Microsoft Cognitive Services”, found at [http://go.microsoft.com/fwlink/?LinkId=698895](http://go.microsoft.com/fwlink/?LinkId=698895).

[[package]]
name = "async-generator"
version = "1.10"
description = "Async generators and context managers for Python 3.5+"
category = "main"
optional = false
python-versions = ">=3.5"

[[package]]
name = "attrs"
version = "21.4.0"
description = "Classes Without Boilerplate"
category = "main"
optional = false
python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"

[package.extras]
dev = ["coverage[toml] (>=5.0.2)", "hypothesis", "pympler", "pytest (>=4.3.0)", "six", "mypy", "pytest-mypy-plugins", "zope.interface", "furo", "sphinx", "sphinx-notfound-page", "pre-commit", "cloudpickle"]
docs = ["furo", "sphinx", "zope.interface", "sphinx-notfound-page"]
tests = ["coverage[toml] (>=5.0.2)", "hypothesis", "pympler", "pytest (>=4.3.0)", "six", "mypy", "pytest-mypy-plugins", "zope.interface", "cloudpickle"]
tests_no_zope = ["coverage[toml] (>=5.0.2)", "hypothesis", "pympler", "pytest (>=4.3.0)", "six", "mypy", "pytest-mypy-plugins", "cloudpickle"]

[[package]]
name = "certifi"
version = "2021.10.8"
description = "Python package for providing Mozilla's CA Bundle."
category = "main"
optional = false
python-versions = "*"

[[package]]
name = "cffi"
version = "1.15.0"
description = "Foreign Function Interface for Python calling C code."
category = "main"
optional = false
python-versions = "*"

[package.dependencies]
pycparser = "*"

[[package]]
name = "cryptography"
version = "36.0.1"
description = "cryptography is a package which provides cryptographic recipes and primitives to Python developers."
category = "main"
optional = false
python-versions = ">=3.6"

[package.dependencies]
cffi = ">=1.12"

[package.extras]
docs = ["sphinx (>=1.6.5,!=1.8.0,!=3.1.0,!=3.1.1)", "sphinx-rtd-theme"]
docstest = ["pyenchant (>=1.6.11)", "twine (>=1.12.0)", "sphinxcontrib-spelling (>=4.0.1)"]
pep8test = ["black", "flake8", "flake8-import-order", "pep8-naming"]
sdist = ["setuptools_rust (>=0.11.4)"]
ssh = ["bcrypt (>=3.1.5)"]
test = ["pytest (>=6.2.0)", "pytest-cov", "pytest-subtests", "pytest-xdist", "pretend", "iso8601", "pytz", "hypothesis (>=1.11.4,!=3.79.2)"]

[[package]]
name = "h11"
version = "0.12.0"
description = "A pure-Python, bring-your-own-I/O implementation of HTTP/1.1"
category = "main"
optional = false
python-versions = ">=3.6"

[[package]]
name = "idna"
version = "3.3"
description = "Internationalized Domain Names in Applications (IDNA)"
category = "main"
optional = false
python-versions = ">=3.5"

[[package]]
name = "outcome"
version = "1.1.0"
description = "Capture the outcome of Python function calls."
category = "main"
optional = false
python-versions = ">=3.6"

[package.dependencies]
attrs = ">=19.2.0"

[[package]]
name = "pycparser"
version = "2.21"
description = "C parser in Python"
category = "main"
optional = false
python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"

[[package]]
name = "pyopenssl"
version = "21.0.0"
description = "Python wrapper module around the OpenSSL library"
category = "main"
optional = false
python-versions = ">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*"

[package.dependencies]
cryptography = ">=3.3"
six = ">=1.5.2"

[package.extras]
docs = ["sphinx", "sphinx-rtd-theme"]
test = ["flaky", "pretend", "pytest (>=3.0.1)"]

[[package]]
name = "selenium"
version = "4.1.0"
description = ""
category = "main"
optional = false
python-versions = "~=3.7"

[package.dependencies]
trio = ">=0.17,<1.0"
trio-websocket = ">=0.9,<1.0"
urllib3 = {version = ">=1.26,<2.0", extras = ["secure"]}

[[package]]
name = "six"
version = "1.16.0"
description = "Python 2 and 3 compatibility utilities"
category = "main"
optional = false
python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"

[[package]]
name = "sniffio"
version = "1.2.0"
description = "Sniff out which async library your code is running under"
category = "main"
optional = false
python-versions = ">=3.5"

[[package]]
name = "sortedcontainers"
version = "2.4.0"
description = "Sorted Containers -- Sorted List, Sorted Dict, Sorted Set"
category = "main"
optional = false
python-versions = "*"

[[package]]
name = "trio"
version = "0.19.0"
description = "A friendly Python library for async concurrency and I/O"
category = "main"
optional = false
python-versions = ">=3.6"

[package.dependencies]
async-generator = ">=1.9"
attrs = ">=19.2.0"
cffi = {version = ">=1.14", markers = "os_name == \"nt\" and implementation_name != \"pypy\""}
idna = "*"
outcome = "*"
sniffio = "*"
sortedcontainers = "*"

[[package]]
name = "trio-websocket"
version = "0.9.2"
description = "WebSocket library for Trio"
category = "main"
optional = false
python-versions = ">=3.5"

[package.dependencies]
async-generator = ">=1.10"
trio = ">=0.11"
wsproto = ">=0.14"

[[package]]
name = "urllib3"
version = "1.26.7"
description = "HTTP library with thread-safe connection pooling, file post, and more."
category = "main"
optional = false
python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, <4"

[package.dependencies]
certifi = {version = "*", optional = true, markers = "extra == \"secure\""}
cryptography = {version = ">=1.3.4", optional = true, markers = "extra == \"secure\""}
idna = {version = ">=2.0.0", optional = true, markers = "extra == \"secure\""}
pyOpenSSL = {version = ">=0.14", optional = true, markers = "extra == \"secure\""}

[package.extras]
brotli = ["brotlipy (>=0.6.0)"]
secure = ["pyOpenSSL (>=0.14)", "cryptography (>=1.3.4)", "idna (>=2.0.0)", "certifi", "ipaddress"]
socks = ["PySocks (>=1.5.6,!=1.5.7,<2.0)"]

[[package]]
name = "wsproto"
version = "1.0.0"
description = "WebSockets state-machine based protocol implementation"
category = "main"
optional = false
python-versions = ">=3.6.1"

[package.dependencies]
h11 = ">=0.9.0,<1"

[metadata]
lock-version = "1.1"
python-versions = "^3.8"
content-hash = "f11f641ac9b19bcd85fbfd2ea897f5490efc65862f964d3d3a59f2eaac19a0b9"

[metadata.files]
async-generator = [
    {file = "async_generator-1.10-py3-none-any.whl", hash = "sha256:01c7bf666359b4967d2cda0000cc2e4af16a0ae098cbffcb8472fb9e8ad6585b"},
    {file = "async_generator-1.10.tar.gz", hash = "sha256:6ebb3d106c12920aaae42ccb6f787ef5eefdcdd166ea3d628fa8476abe712144"},
]
attrs = [
    {file = "attrs-21.4.0-py2.py3-none-any.whl", hash = "sha256:2d27e3784d7a565d36ab851fe94887c5eccd6a463168875832a1be79c82828b4"},
    {file = "attrs-21.4.0.tar.gz", hash = "sha256:626ba8234211db98e869df76230a137c4c40a12d72445c45d5f5b716f076e2fd"},
]
certifi = [
    {file = "certifi-2021.10.8-py2.py3-none-any.whl", hash = "sha256:d62a0163eb4c2344ac042ab2bdf75399a71a2d8c7d47eac2e2ee91b9d6339569"},
    {file = "certifi-2021.10.8.tar.gz", hash = "sha256:78884e7c1d4b00ce3cea67b44566851c4343c120abd683433ce934a68ea58872"},
]
cffi = [
    {file = "cffi-1.15.0-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:c2502a1a03b6312837279c8c1bd3ebedf6c12c4228ddbad40912d671ccc8a962"},
    {file = "cffi-1.15.0-cp27-cp27m-manylinux1_i686.whl", hash = "sha256:23cfe892bd5dd8941608f93348c0737e369e51c100d03718f108bf1add7bd6d0"},
    {file = "cffi-1.15.0-cp27-cp27m-manylinux1_x86_64.whl", hash = "sha256:41d45de54cd277a7878919867c0f08b0cf817605e4eb94093e7516505d3c8d14"},
    {file = "cffi-1.15.0-cp27-cp27m-win32.whl", hash = "sha256:4a306fa632e8f0928956a41fa8e1d6243c71e7eb59ffbd165fc0b41e316b2474"},
    {file = "cffi-1.15.0-cp27-cp27m-win_amd64.whl", hash = "sha256:e7022a66d9b55e93e1a845d8c9eba2a1bebd4966cd8bfc25d9cd07d515b33fa6"},
    {file = "cffi-1.15.0-cp27-cp27mu-manylinux1_i686.whl", hash = "sha256:14cd121ea63ecdae71efa69c15c5543a4b5fbcd0bbe2aad864baca0063cecf27"},
    {file = "cffi-1.15.0-cp27-cp27mu-manylinux1_x86_64.whl", hash = "sha256:d4d692a89c5cf08a8557fdeb329b82e7bf609aadfaed6c0d79f5a449a3c7c023"},
    {file = "cffi-1.15.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:0104fb5ae2391d46a4cb082abdd5c69ea4eab79d8d44eaaf79f1b1fd806ee4c2"},
    {file = "cffi-1.15.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:91ec59c33514b7c7559a6acda53bbfe1b283949c34fe7440bcf917f96ac0723e"},
    {file = "cffi-1.15.0-cp310-cp310-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:f5c7150ad32ba43a07c4479f40241756145a1f03b43480e058cfd862bf5041c7"},
    {file = "cffi-1.15.0-cp310-cp310-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:00c878c90cb53ccfaae6b8bc18ad05d2036553e6d9d1d9dbcf323bbe83854ca3"},
    {file = "cffi-1.15.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:abb9a20a72ac4e0fdb50dae135ba5e77880518e742077ced47eb1499e29a443c"},
    {file = "cffi-1.15.0-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:a5263e363c27b653a90078143adb3d076c1a748ec9ecc78ea2fb916f9b861962"},
    {file = "cffi-1.15.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:f54a64f8b0c8ff0b64d18aa76675262e1700f3995182267998c31ae974fbc382"},
    {file = "cffi-1.15.0-cp310-cp310-win32.whl", hash = "sha256:c21c9e3896c23007803a875460fb786118f0cdd4434359577ea25eb556e34c55"},
    {file = "cffi-1.15.0-cp310-cp310-win_amd64.whl", hash = "sha256:5e069f72d497312b24fcc02073d70cb989045d1c91cbd53979366077959933e0"},
    {file = "cffi-1.15.0-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:64d4ec9f448dfe041705426000cc13e34e6e5bb13736e9fd62e34a0b0c41566e"},
    {file = "cffi-1.15.0-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2756c88cbb94231c7a147402476be2c4df2f6078099a6f4a480d239a8817ae39"},
    {file = "cffi-1.15.0-cp36-cp36m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3b96a311ac60a3f6be21d2572e46ce67f09abcf4d09344c49274eb9e0bf345fc"},
    {file = "cffi-1.15.0-cp36-cp36m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:75e4024375654472cc27e91cbe9eaa08567f7fbdf822638be2814ce059f58032"},
    {file = "cffi-1.15.0-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:59888172256cac5629e60e72e86598027aca6bf01fa2465bdb676d37636573e8"},
    {file = "cffi-1.15.0-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:27c219baf94952ae9d50ec19651a687b826792055353d07648a5695413e0c605"},
    {file = "cffi-1.15.0-cp36-cp36m-win32.whl", hash = "sha256:4958391dbd6249d7ad855b9ca88fae690783a6be9e86df65865058ed81fc860e"},
    {file = "cffi-1.15.0-cp36-cp36m-win_amd64.whl", hash = "sha256:f6f824dc3bce0edab5f427efcfb1d63ee75b6fcb7282900ccaf925be84efb0fc"},
    {file = "cffi-1.15.0-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:06c48159c1abed75c2e721b1715c379fa3200c7784271b3c46df01383b593636"},
    {file = "cffi-1.15.0-cp37-cp37m-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:c2051981a968d7de9dd2d7b87bcb9c939c74a34626a6e2f8181455dd49ed69e4"},
    {file = "cffi-1.15.0-cp37-cp37m-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:fd8a250edc26254fe5b33be00402e6d287f562b6a5b2152dec302fa15bb3e997"},
    {file = "cffi-1.15.0-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:91d77d2a782be4274da750752bb1650a97bfd8f291022b379bb8e01c66b4e96b"},
    {file = "cffi-1.15.0-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:45db3a33139e9c8f7c09234b5784a5e33d31fd6907800b316decad50af323ff2"},
    {file = "cffi-1.15.0-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:263cc3d821c4ab2213cbe8cd8b355a7f72a8324577dc865ef98487c1aeee2bc7"},
    {file = "cffi-1.15.0-cp37-cp37m-win32.whl", hash = "sha256:17771976e82e9f94976180f76468546834d22a7cc404b17c22df2a2c81db0c66"},
    {file = "cffi-1.15.0-cp37-cp37m-win_amd64.whl", hash = "sha256:3415c89f9204ee60cd09b235810be700e993e343a408693e80ce7f6a40108029"},
    {file = "cffi-1.15.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:4238e6dab5d6a8ba812de994bbb0a79bddbdf80994e4ce802b6f6f3142fcc880"},
    {file = "cffi-1.15.0-cp38-cp38-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:0808014eb713677ec1292301ea4c81ad277b6cdf2fdd90fd540af98c0b101d20"},
    {file = "cffi-1.15.0-cp38-cp38-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:57e9ac9ccc3101fac9d6014fba037473e4358ef4e89f8e181f8951a2c0162024"},
    {file = "cffi-1.15.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8b6c2ea03845c9f501ed1313e78de148cd3f6cad741a75d43a29b43da27f2e1e"},
    {file = "cffi-1.15.0-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:10dffb601ccfb65262a27233ac273d552ddc4d8ae1bf93b21c94b8511bffe728"},
    {file = "cffi-1.15.0-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:786902fb9ba7433aae840e0ed609f45c7bcd4e225ebb9c753aa39725bb3e6ad6"},
    {file = "cffi-1.15.0-cp38-cp38-win32.whl", hash = "sha256:da5db4e883f1ce37f55c667e5c0de439df76ac4cb55964655906306918e7363c"},
    {file = "cffi-1.15.0-cp38-cp38-win_amd64.whl", hash = "sha256:181dee03b1170ff1969489acf1c26533710231c58f95534e3edac87fff06c443"},
    {file = "cffi-1.15.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:45e8636704eacc432a206ac7345a5d3d2c62d95a507ec70d62f23cd91770482a"},
    {file = "cffi-1.15.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:31fb708d9d7c3f49a60f04cf5b119aeefe5644daba1cd2a0fe389b674fd1de37"},
    {file = "cffi-1.15.0-cp39-cp39-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:6dc2737a3674b3e344847c8686cf29e500584ccad76204efea14f451d4cc669a"},
    {file = "cffi-1.15.0-cp39-cp39-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:74fdfdbfdc48d3f47148976f49fab3251e550a8720bebc99bf1483f5bfb5db3e"},
    {file = "cffi-1.15.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ffaa5c925128e29efbde7301d8ecaf35c8c60ffbcd6a1ffd3a552177c8e5e796"},
    {file = "cffi-1.15.0-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3f7d084648d77af029acb79a0ff49a0ad7e9d09057a9bf46596dac9514dc07df"},
    {file = "cffi-1.15.0-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:ef1f279350da2c586a69d32fc8733092fd32cc8ac95139a00377841f59a3f8d8"},
    {file = "cffi-1.15.0-cp39-cp39-win32.whl", hash = "sha256:2a23af14f408d53d5e6cd4e3d9a24ff9e05906ad574822a10563efcef137979a"},
    {file = "cffi-1.15.0-cp39-cp39-win_amd64.whl", hash = "sha256:3773c4d81e6e818df2efbc7dd77325ca0dcb688116050fb2b3011218eda36139"},
    {file = "cffi-1.15.0.tar.gz", hash = "sha256:920f0d66a896c2d99f0adbb391f990a84091179542c205fa53ce5787aff87954"},
]
cryptography = [
    {file = "cryptography-36.0.1-cp36-abi3-macosx_10_10_universal2.whl", hash = "sha256:73bc2d3f2444bcfeac67dd130ff2ea598ea5f20b40e36d19821b4df8c9c5037b"},
    {file = "cryptography-36.0.1-cp36-abi3-macosx_10_10_x86_64.whl", hash = "sha256:2d87cdcb378d3cfed944dac30596da1968f88fb96d7fc34fdae30a99054b2e31"},
    {file = "cryptography-36.0.1-cp36-abi3-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:74d6c7e80609c0f4c2434b97b80c7f8fdfaa072ca4baab7e239a15d6d70ed73a"},
    {file = "cryptography-36.0.1-cp36-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:6c0c021f35b421ebf5976abf2daacc47e235f8b6082d3396a2fe3ccd537ab173"},
    {file = "cryptography-36.0.1-cp36-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5d59a9d55027a8b88fd9fd2826c4392bd487d74bf628bb9d39beecc62a644c12"},
    {file = "cryptography-36.0.1-cp36-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0a817b961b46894c5ca8a66b599c745b9a3d9f822725221f0e0fe49dc043a3a3"},
    {file = "cryptography-36.0.1-cp36-abi3-manylinux_2_24_x86_64.whl", hash = "sha256:94ae132f0e40fe48f310bba63f477f14a43116f05ddb69d6fa31e93f05848ae2"},
    {file = "cryptography-36.0.1-cp36-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:7be0eec337359c155df191d6ae00a5e8bbb63933883f4f5dffc439dac5348c3f"},
    {file = "cryptography-36.0.1-cp36-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:e0344c14c9cb89e76eb6a060e67980c9e35b3f36691e15e1b7a9e58a0a6c6dc3"},
    {file = "cryptography-36.0.1-cp36-abi3-win32.whl", hash = "sha256:4caa4b893d8fad33cf1964d3e51842cd78ba87401ab1d2e44556826df849a8ca"},
    {file = "cryptography-36.0.1-cp36-abi3-win_amd64.whl", hash = "sha256:391432971a66cfaf94b21c24ab465a4cc3e8bf4a939c1ca5c3e3a6e0abebdbcf"},
    {file = "cryptography-36.0.1-pp37-pypy37_pp73-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:bb5829d027ff82aa872d76158919045a7c1e91fbf241aec32cb07956e9ebd3c9"},
    {file = "cryptography-36.0.1-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ebc15b1c22e55c4d5566e3ca4db8689470a0ca2babef8e3a9ee057a8b82ce4b1"},
    {file = "cryptography-36.0.1-pp37-pypy37_pp73-manylinux_2_24_x86_64.whl", hash = "sha256:596f3cd67e1b950bc372c33f1a28a0692080625592ea6392987dba7f09f17a94"},
    {file = "cryptography-36.0.1-pp38-pypy38_pp73-macosx_10_10_x86_64.whl", hash = "sha256:30ee1eb3ebe1644d1c3f183d115a8c04e4e603ed6ce8e394ed39eea4a98469ac"},
    {file = "cryptography-36.0.1-pp38-pypy38_pp73-manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:ec63da4e7e4a5f924b90af42eddf20b698a70e58d86a72d943857c4c6045b3ee"},
    {file = "cryptography-36.0.1-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ca238ceb7ba0bdf6ce88c1b74a87bffcee5afbfa1e41e173b1ceb095b39add46"},
    {file = "cryptography-36.0.1-pp38-pypy38_pp73-manylinux_2_24_x86_64.whl", hash = "sha256:ca28641954f767f9822c24e927ad894d45d5a1e501767599647259cbf030b903"},
    {file = "cryptography-36.0.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:39bdf8e70eee6b1c7b289ec6e5d84d49a6bfa11f8b8646b5b3dfe41219153316"},
    {file = "cryptography-36.0.1.tar.gz", hash = "sha256:53e5c1dc3d7a953de055d77bef2ff607ceef7a2aac0353b5d630ab67f7423638"},
]
h11 = [
    {file = "h11-0.12.0-py3-none-any.whl", hash = "sha256:36a3cb8c0a032f56e2da7084577878a035d3b61d104230d4bd49c0c6b555a9c6"},
    {file = "h11-0.12.0.tar.gz", hash = "sha256:47222cb6067e4a307d535814917cd98fd0a57b6788ce715755fa2b6c28b56042"},
]
idna = [
    {file = "idna-3.3-py3-none-any.whl", hash = "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff"},
    {file = "idna-3.3.tar.gz", hash = "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"},
]
outcome = [
    {file = "outcome-1.1.0-py2.py3-none-any.whl", hash = "sha256:c7dd9375cfd3c12db9801d080a3b63d4b0a261aa996c4c13152380587288d958"},
    {file = "outcome-1.1.0.tar.gz", hash = "sha256:e862f01d4e626e63e8f92c38d1f8d5546d3f9cce989263c521b2e7990d186967"},
]
pycparser = [
    {file = "pycparser-2.21-py2.py3-none-any.whl", hash = "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9"},
    {file = "pycparser-2.21.tar.gz", hash = "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"},
]
pyopenssl = [
    {file = "pyOpenSSL-21.0.0-py2.py3-none-any.whl", hash = "sha256:8935bd4920ab9abfebb07c41a4f58296407ed77f04bd1a92914044b848ba1ed6"},
    {file = "pyOpenSSL-21.0.0.tar.gz", hash = "sha256:5e2d8c5e46d0d865ae933bef5230090bdaf5506281e9eec60fa250ee80600cb3"},
]
selenium = [
    {file = "selenium-4.1.0-py3-none-any.whl", hash = "sha256:27e7b64df961d609f3d57237caa0df123abbbe22d038f2ec9e332fb90ec1a939"},
]
six = [
    {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
    {file = "six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
]
sniffio = [
    {file = "sniffio-1.2.0-py3-none-any.whl", hash = "sha256:471b71698eac1c2112a40ce2752bb2f4a4814c22a54a3eed3676bc0f5ca9f663"},
    {file = "sniffio-1.2.0.tar.gz", hash = "sha256:c4666eecec1d3f50960c6bdf61ab7bc350648da6c126e3cf6898d8cd4ddcd3de"},
]
sortedcontainers = [
    {file = "sortedcontainers-2.4.0-py2.py3-none-any.whl", hash = "sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0"},
    {file = "sortedcontainers-2.4.0.tar.gz", hash = "sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88"},
]
trio = [
    {file = "trio-0.19.0-py3-none-any.whl", hash = "sha256:c27c231e66336183c484fbfe080fa6cc954149366c15dc21db8b7290081ec7b8"},
    {file = "trio-0.19.0.tar.gz", hash = "sha256:895e318e5ec5e8cea9f60b473b6edb95b215e82d99556a03eb2d20c5e027efe1"},
]
trio-websocket = [
    {file = "trio-websocket-0.9.2.tar.gz", hash = "sha256:a3d34de8fac26023eee701ed1e7bf4da9a8326b61a62934ec9e53b64970fd8fe"},
    {file = "trio_websocket-0.9.2-py3-none-any.whl", hash = "sha256:5b558f6e83cc20a37c3b61202476c5295d1addf57bd65543364e0337e37ed2bc"},
]
urllib3 = [
    {file = "urllib3-1.26.7-py2.py3-none-any.whl", hash = "sha256:c4fdf4019605b6e5423637e01bc9fe4daef873709a7973e195ceba0a62bbc844"},
    {file = "urllib3-1.26.7.tar.gz", hash = "sha256:4987c65554f7a2dbf30c18fd48778ef124af6fab771a377103da0585e2336ece"},
]
wsproto = [
    {file = "wsproto-1.0.0-py3-none-any.whl", hash = "sha256:d8345d1808dd599b5ffb352c25a367adb6157e664e140dbecba3f9bc007edb9f"},
    {file = "wsproto-1.0.0.tar.gz", hash = "sha256:868776f8456997ad0d9720f7322b746bbe9193751b5b290b7f924659377c8c38"},
]


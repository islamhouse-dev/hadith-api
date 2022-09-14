# hadith-api
HadeethEnc.com official API, providing islamic hadith contents in more than 20 languages.

# Project: HadeethEnc.com/API/v1
HadeethEnc.com API

## End-point: languages
https://hadeethenc.com/api/v1/languages

List all available languages for HadeethEnc.com

This endpoint returns json object containing all available languages with their iso codes and native names.
### Method: GET
>```
>https://hadeethenc.com/api/v1/languages
>```
### Response: 200
```json
[
    {
        "code": "ar",
        "native": "عربي"
    },
    {
        "code": "en",
        "native": "English"
    },
    {
        "code": "fr",
        "native": "Français"
    },
    {
        "code": "es",
        "native": "Español"
    },
    {
        "code": "tr",
        "native": "Türkçe"
    },
    {
        "code": "ur",
        "native": "اردو"
    },
    {
        "code": "id",
        "native": "Indonesia"
    },
    {
        "code": "bs",
        "native": "Bosanski"
    },
    {
        "code": "ru",
        "native": "Русский"
    },
    {
        "code": "bn",
        "native": "বাংলা ভাষা"
    },
    {
        "code": "zh",
        "native": "中文"
    },
    {
        "code": "fa",
        "native": "فارسی"
    },
    {
        "code": "tl",
        "native": "Tagalog"
    },
    {
        "code": "hi",
        "native": "हिन्दी"
    },
    {
        "code": "vi",
        "native": "Tiếng Việt"
    },
    {
        "code": "si",
        "native": "සිංහල"
    },
    {
        "code": "ug",
        "native": "ئۇيغۇرچە"
    }
]
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: /categories/list/?language={language_code}
https://hadeethenc.com/api/v1/categories/list/?language=en

List all categories by language code.

This endpoint accepts language iso code and returns array of json objects each object represents a category.
### Method: GET
>```
>https://hadeethenc.com/api/v1/categories/list/?language=en
>```
### Query Params

|Param|value|
|---|---|
|language|en|


### Response: 200
```json
[
    {
        "id": "1",
        "title": "The Noble Qur'an and Qur'anic Sciences",
        "hadeeths_count": "59",
        "parent_id": null
    },
    {
        "id": "2",
        "title": "The Hadith and Hadith Sciences",
        "hadeeths_count": "5",
        "parent_id": null
    },
    {
        "id": "3",
        "title": "The Creed",
        "hadeeths_count": "441",
        "parent_id": null
    },
    {
        "id": "4",
        "title": "Jurisprudence and Juristic Principles",
        "hadeeths_count": "1347",
        "parent_id": null
    },
    {
        "id": "5",
        "title": "Virtues and Manners",
        "hadeeths_count": "822",
        "parent_id": null
    },
    {
        "id": "6",
        "title": "Da‘wah and Hisbah",
        "hadeeths_count": "98",
        "parent_id": null
    },
    {
        "id": "7",
        "title": "Seerah and History",
        "hadeeths_count": "228",
        "parent_id": null
    },
    {
        "id": "8",
        "title": "Revelation and Collection of the Qur'an",
        "hadeeths_count": "9",
        "parent_id": "1"
    },
    {
        "id": "9",
        "title": "Modes of Qur'anic Recitation and Tajweed",
        "hadeeths_count": "4",
        "parent_id": "1"
    },
    {
        "id": "10",
        "title": "Qur'anic Exegesis",
        "hadeeths_count": "10",
        "parent_id": "1"
    },
    {
        "id": "11",
        "title": "General Qur'anic Topics",
        "hadeeths_count": "12",
        "parent_id": "1"
    },
    {
        "id": "12",
        "title": "Excellence of the Qur'an",
        "hadeeths_count": "24",
        "parent_id": "1"
    },
    {
        "id": "14",
        "title": "Occasions of Revelation",
        "hadeeths_count": "1",
        "parent_id": "8"
    },
    {
        "id": "16",
        "title": "Abrogating and Abrogated Verses",
        "hadeeths_count": "1",
        "parent_id": "8"
    },
    {
        "id": "17",
        "title": "Collecting the Qur'an",
        "hadeeths_count": "2",
        "parent_id": "8"
    },
    {
        "id": "18",
        "title": "Seven Modes of the Qur'anic Revelation",
        "hadeeths_count": "3",
        "parent_id": "9"
    },
    {
        "id": "20",
        "title": "Science of Tajweed",
        "hadeeths_count": "1",
        "parent_id": "9"
    },
    {
        "id": "29",
        "title": "Rulings of the Qur'an and Codices",
        "hadeeths_count": "3",
        "parent_id": "11"
    },
    {
        "id": "31",
        "title": "Manners of Reading and Memorizing the Qur'an",
        "hadeeths_count": "4",
        "parent_id": "11"
    },
    {
        "id": "32",
        "title": "Refuting Allegations against the Qur'an",
        "hadeeths_count": "4",
        "parent_id": "11"
    },
    {
        "id": "38",
        "title": "Inference from the Qur'an",
        "hadeeths_count": "1",
        "parent_id": "11"
    },
    {
        "id": "39",
        "title": "Merit of Taking Care of the Qur'an",
        "hadeeths_count": "14",
        "parent_id": "12"
    },
    {
        "id": "40",
        "title": "Virtues of Surahs and Verses",
        "hadeeths_count": "10",
        "parent_id": "12"
    },
    {
        "id": "44",
        "title": "General Sunnah Topics",
        "hadeeths_count": "5",
        "parent_id": "2"
    },
    {
        "id": "56",
        "title": "Significance and Status of the Sunnah",
        "hadeeths_count": "4",
        "parent_id": "44"
    },
    {
        "id": "57",
        "title": "Writing the Sunnah",
        "hadeeths_count": "1",
        "parent_id": "44"
    },
    {
        "id": "59",
        "title": "Belief in Allah the Mighty and Majestic",
        "hadeeths_count": "127",
        "parent_id": "3"
    },
    {
        "id": "60",
        "title": "Belief in the Angels",
        "hadeeths_count": "31",
        "parent_id": "3"
    },
    {
        "id": "61",
        "title": "Belief in the Revealed Books",
        "hadeeths_count": "2",
        "parent_id": "3"
    },
    {
        "id": "62",
        "title": "Belief in the Messengers",
        "hadeeths_count": "41",
        "parent_id": "3"
    },
    {
        "id": "63",
        "title": "Belief in the Last Day",
        "hadeeths_count": "91",
        "parent_id": "3"
    },
    {
        "id": "64",
        "title": "Belief in the Divine Decree and Fate",
        "hadeeths_count": "19",
        "parent_id": "3"
    },
    {
        "id": "65",
        "title": "Names and Rulings",
        "hadeeths_count": "61",
        "parent_id": "3"
    },
    {
        "id": "66",
        "title": "The Companions",
        "hadeeths_count": "36",
        "parent_id": "3"
    },
    {
        "id": "67",
        "title": "The Prophet's Family",
        "hadeeths_count": "14",
        "parent_id": "3"
    },
    {
        "id": "68",
        "title": "Allegiance and Dissociation",
        "hadeeths_count": "15",
        "parent_id": "3"
    },
    {
        "id": "71",
        "title": "Sects and Schools",
        "hadeeths_count": "1",
        "parent_id": "3"
    },
    {
        "id": "72",
        "title": "Oneness of Allah's Lordship",
        "hadeeths_count": "6",
        "parent_id": "59"
    },
    {
        "id": "73",
        "title": "Oneness of Allah's Worship",
        "hadeeths_count": "43",
        "parent_id": "59"
    },
    {
        "id": "74",
        "title": "Oneness of Allah's Names and Attributes",
        "hadeeths_count": "73",
        "parent_id": "59"
    },
    {
        "id": "75",
        "title": "The Angels",
        "hadeeths_count": "21",
        "parent_id": "60"
    },
    {
        "id": "76",
        "title": "The Jinn",
        "hadeeths_count": "6",
        "parent_id": "60"
    },
    {
        "id": "78",
        "title": "The Qur'an",
        "hadeeths_count": "1",
        "parent_id": "61"
    },
    {
        "id": "79",
        "title": "Prophethood",
        "hadeeths_count": "2",
        "parent_id": "62"
    },
    {
        "id": "80",
        "title": "Pre-Islamic Prophets and Messengers, peace be upon them",
        "hadeeths_count": "23",
        "parent_id": "62"
    },
    {
        "id": "81",
        "title": "Our Prophet Muhammad, may Allah's peace and blessings be upon him",
        "hadeeths_count": "14",
        "parent_id": "62"
    },
    {
        "id": "82",
        "title": "Miracles of the Pious Allies of Allah",
        "hadeeths_count": "2",
        "parent_id": "62"
    },
    {
        "id": "83",
        "title": "The Barzakh Life (After death Period)",
        "hadeeths_count": "10",
        "parent_id": "63"
    },
    {
        "id": "84",
        "title": "Portents of the Hour",
        "hadeeths_count": "29",
        "parent_id": "63"
    },
    {
        "id": "85",
        "title": "The Hereafter Life",
        "hadeeths_count": "39",
        "parent_id": "63"
    },
    {
        "id": "86",
        "title": "Levels of Divine Decree and Fate",
        "hadeeths_count": "7",
        "parent_id": "64"
    },
    {
        "id": "87",
        "title": "Issues of Divine Decree and Fate",
        "hadeeths_count": "9",
        "parent_id": "64"
    },
    {
        "id": "88",
        "title": "Islam",
        "hadeeths_count": "8",
        "parent_id": "65"
    },
    {
        "id": "89",
        "title": "Nullifiers of Islam",
        "hadeeths_count": "5",
        "parent_id": "65"
    },
    {
        "id": "90",
        "title": "Issues of Pre-Islamic Era",
        "hadeeths_count": "8",
        "parent_id": "65"
    },
    {
        "id": "92",
        "title": "Increase and Decrease of Faith",
        "hadeeths_count": "4",
        "parent_id": "65"
    },
    {
        "id": "93",
        "title": "Exceptions in Faith",
        "hadeeths_count": "1",
        "parent_id": "65"
    },
    {
        "id": "94",
        "title": "Branches of Faith",
        "hadeeths_count": "3",
        "parent_id": "65"
    },
    {
        "id": "96",
        "title": "Disbelief",
        "hadeeths_count": "3",
        "parent_id": "65"
    },
    {
        "id": "97",
        "title": "Polytheism",
        "hadeeths_count": "14",
        "parent_id": "65"
    },
    {
        "id": "98",
        "title": "Hypocrisy",
        "hadeeths_count": "7",
        "parent_id": "65"
    },
    {
        "id": "99",
        "title": "Immorality",
        "hadeeths_count": "3",
        "parent_id": "65"
    },
    {
        "id": "100",
        "title": "Religious Innovation",
        "hadeeths_count": "4",
        "parent_id": "65"
    },
    {
        "id": "101",
        "title": "Merit of the Companions",
        "hadeeths_count": "28",
        "parent_id": "66"
    },
    {
        "id": "102",
        "title": "Belief in the the Companions",
        "hadeeths_count": "2",
        "parent_id": "66"
    },
    {
        "id": "103",
        "title": "Degrees of the Companions",
        "hadeeths_count": "6",
        "parent_id": "66"
    },
    {
        "id": "105",
        "title": "Merit of the Prophet's Family",
        "hadeeths_count": "5",
        "parent_id": "67"
    },
    {
        "id": "106",
        "title": "Merit of the Mothers of the Believers",
        "hadeeths_count": "4",
        "parent_id": "67"
    },
    {
        "id": "107",
        "title": "Belief in the Prophet's Family",
        "hadeeths_count": "1",
        "parent_id": "67"
    },
    {
        "id": "108",
        "title": "Rights of the Prophet's Family",
        "hadeeths_count": "4",
        "parent_id": "67"
    },
    {
        "id": "109",
        "title": "Rulings of Allegiance and Dissociation",
        "hadeeths_count": "5",
        "parent_id": "68"
    },
    {
        "id": "110",
        "title": "Forbidden Emulation",
        "hadeeths_count": "6",
        "parent_id": "68"
    },
    {
        "id": "111",
        "title": "Emigration and its Rulings",
        "hadeeths_count": "2",
        "parent_id": "68"
    },
    {
        "id": "112",
        "title": "Desertion and its Conditions",
        "hadeeths_count": "2",
        "parent_id": "68"
    },
    {
        "id": "119",
        "title": "Old Sects and Schools",
        "hadeeths_count": "1",
        "parent_id": "71"
    },
    {
        "id": "121",
        "title": "Jurisprudence of Acts of Worship",
        "hadeeths_count": "832",
        "parent_id": "4"
    },
    {
        "id": "122",
        "title": "Jurisprudence of Transactions",
        "hadeeths_count": "107",
        "parent_id": "4"
    },
    {
        "id": "123",
        "title": "Religious Obligations",
        "hadeeths_count": "10",
        "parent_id": "4"
    },
    {
        "id": "124",
        "title": "Family Jurisprudence",
        "hadeeths_count": "225",
        "parent_id": "4"
    },
    {
        "id": "125",
        "title": "Spiritual and Physical Therapy",
        "hadeeths_count": "21",
        "parent_id": "4"
    },
    {
        "id": "126",
        "title": "Foods and Drinks",
        "hadeeths_count": "41",
        "parent_id": "4"
    },
    {
        "id": "127",
        "title": "Crimes",
        "hadeeths_count": "25",
        "parent_id": "4"
    },
    {
        "id": "128",
        "title": "Prescribed Punishments",
        "hadeeths_count": "49",
        "parent_id": "4"
    },
    {
        "id": "129",
        "title": "Judiciary",
        "hadeeths_count": "21",
        "parent_id": "4"
    },
    {
        "id": "132",
        "title": "Principles of Islamic Jurisprudence",
        "hadeeths_count": "14",
        "parent_id": "4"
    },
    {
        "id": "133",
        "title": "Purification",
        "hadeeths_count": "151",
        "parent_id": "121"
    },
    {
        "id": "134",
        "title": "Prayer",
        "hadeeths_count": "383",
        "parent_id": "121"
    },
    {
        "id": "135",
        "title": "Funerals",
        "hadeeths_count": "35",
        "parent_id": "121"
    },
    {
        "id": "136",
        "title": "Zakah",
        "hadeeths_count": "39",
        "parent_id": "121"
    },
    {
        "id": "137",
        "title": "Fasting",
        "hadeeths_count": "60",
        "parent_id": "121"
    },
    {
        "id": "138",
        "title": "Hajj and ‘Umrah",
        "hadeeths_count": "66",
        "parent_id": "121"
    },
    {
        "id": "139",
        "title": "Jihad",
        "hadeeths_count": "98",
        "parent_id": "121"
    },
    {
        "id": "140",
        "title": "Sales",
        "hadeeths_count": "21",
        "parent_id": "122"
    },
    {
        "id": "141",
        "title": "Conditions of Sale",
        "hadeeths_count": "1",
        "parent_id": "140"
    },
    {
        "id": "142",
        "title": "Sale-Related Stipulations",
        "hadeeths_count": "2",
        "parent_id": "140"
    },
    {
        "id": "143",
        "title": "Selling Assets and Fruits",
        "hadeeths_count": "3",
        "parent_id": "140"
    },
    {
        "id": "144",
        "title": "Advance Payment",
        "hadeeths_count": "1",
        "parent_id": "122"
    },
    {
        "id": "145",
        "title": "Usury",
        "hadeeths_count": "5",
        "parent_id": "122"
    },
    {
        "id": "146",
        "title": "Loan",
        "hadeeths_count": "3",
        "parent_id": "122"
    },
    {
        "id": "147",
        "title": "Mortgage",
        "hadeeths_count": "1",
        "parent_id": "122"
    },
    {
        "id": "148",
        "title": "Collateral and Surety",
        "hadeeths_count": "1",
        "parent_id": "122"
    },
    {
        "id": "150",
        "title": "Conciliation and Neighborhood Rulings",
        "hadeeths_count": "4",
        "parent_id": "122"
    },
    {
        "id": "151",
        "title": "Interdiction",
        "hadeeths_count": "1",
        "parent_id": "122"
    },
    {
        "id": "153",
        "title": "Partnership",
        "hadeeths_count": "1",
        "parent_id": "122"
    },
    {
        "id": "154",
        "title": "Sharecropping",
        "hadeeths_count": "3",
        "parent_id": "122"
    },
    {
        "id": "156",
        "title": "Racing and Gambling",
        "hadeeths_count": "3",
        "parent_id": "122"
    },
    {
        "id": "158",
        "title": "Usurpation",
        "hadeeths_count": "2",
        "parent_id": "122"
    },
    {
        "id": "159",
        "title": "Preemption",
        "hadeeths_count": "1",
        "parent_id": "122"
    },
    {
        "id": "163",
        "title": "Found Item and Foundling",
        "hadeeths_count": "2",
        "parent_id": "122"
    },
    {
        "id": "164",
        "title": "Endowment",
        "hadeeths_count": "4",
        "parent_id": "122"
    },
    {
        "id": "165",
        "title": "Gift",
        "hadeeths_count": "9",
        "parent_id": "122"
    },
    {
        "id": "166",
        "title": "Bequest",
        "hadeeths_count": "4",
        "parent_id": "122"
    },
    {
        "id": "167",
        "title": "Manumission",
        "hadeeths_count": "18",
        "parent_id": "122"
    },
    {
        "id": "169",
        "title": "Oaths and Vows",
        "hadeeths_count": "23",
        "parent_id": "122"
    },
    {
        "id": "173",
        "title": "Conditions of Inheritance",
        "hadeeths_count": "1",
        "parent_id": "123"
    },
    {
        "id": "174",
        "title": "Impediments of Inheritance",
        "hadeeths_count": "4",
        "parent_id": "123"
    },
    {
        "id": "175",
        "title": "Sharers",
        "hadeeths_count": "2",
        "parent_id": "123"
    },
    {
        "id": "176",
        "title": "Agnates",
        "hadeeths_count": "1",
        "parent_id": "123"
    },
    {
        "id": "182",
        "title": "Inheritance Shares of Blood Relatives",
        "hadeeths_count": "1",
        "parent_id": "123"
    },
    {
        "id": "183",
        "title": "Inheritance Shares of Embryos",
        "hadeeths_count": "1",
        "parent_id": "123"
    },
    {
        "id": "191",
        "title": "Marriage",
        "hadeeths_count": "81",
        "parent_id": "124"
    },
    {
        "id": "192",
        "title": "Divorce",
        "hadeeths_count": "19",
        "parent_id": "124"
    },
    {
        "id": "193",
        "title": "Remarriage with One's Divorcee",
        "hadeeths_count": "1",
        "parent_id": "124"
    },
    {
        "id": "194",
        "title": "Wife-Initiated Divorce",
        "hadeeths_count": "3",
        "parent_id": "124"
    },
    {
        "id": "195",
        "title": "Oath to Abstain from Intercourse with One's Wife",
        "hadeeths_count": "4",
        "parent_id": "124"
    },
    {
        "id": "196",
        "title": "Zihaar (Likening one's wife to an unmarrriagble woman)",
        "hadeeths_count": "3",
        "parent_id": "124"
    },
    {
        "id": "197",
        "title": "Oath of Condemnation",
        "hadeeths_count": "13",
        "parent_id": "124"
    },
    {
        "id": "198",
        "title": "Waiting Period",
        "hadeeths_count": "15",
        "parent_id": "124"
    },
    {
        "id": "199",
        "title": "Breastfeeding",
        "hadeeths_count": "13",
        "parent_id": "124"
    },
    {
        "id": "200",
        "title": "Custody",
        "hadeeths_count": "3",
        "parent_id": "124"
    },
    {
        "id": "201",
        "title": "Expenses",
        "hadeeths_count": "13",
        "parent_id": "124"
    },
    {
        "id": "202",
        "title": "Clothing and Adornment",
        "hadeeths_count": "10",
        "parent_id": "124"
    },
    {
        "id": "204",
        "title": "Muslim Society",
        "hadeeths_count": "5",
        "parent_id": "124"
    },
    {
        "id": "205",
        "title": "Rulings of Women",
        "hadeeths_count": "32",
        "parent_id": "124"
    },
    {
        "id": "206",
        "title": "Rulings of Newborns",
        "hadeeths_count": "10",
        "parent_id": "124"
    },
    {
        "id": "207",
        "title": "Prophetic Medicine",
        "hadeeths_count": "4",
        "parent_id": "125"
    },
    {
        "id": "208",
        "title": "Rulings of Medication",
        "hadeeths_count": "3",
        "parent_id": "125"
    },
    {
        "id": "211",
        "title": "Ruqyah (Healing and Protective Supplications)",
        "hadeeths_count": "9",
        "parent_id": "125"
    },
    {
        "id": "212",
        "title": "Rulings of Foods and Drinks",
        "hadeeths_count": "6",
        "parent_id": "126"
    },
    {
        "id": "213",
        "title": "Lawful and Unlawful Animals and Birds",
        "hadeeths_count": "16",
        "parent_id": "126"
    },
    {
        "id": "215",
        "title": "Slaughtering",
        "hadeeths_count": "8",
        "parent_id": "126"
    },
    {
        "id": "216",
        "title": "Hunting",
        "hadeeths_count": "6",
        "parent_id": "126"
    },
    {
        "id": "218",
        "title": "Forbidden Drinks",
        "hadeeths_count": "5",
        "parent_id": "126"
    },
    {
        "id": "219",
        "title": "Retribution",
        "hadeeths_count": "12",
        "parent_id": "127"
    },
    {
        "id": "220",
        "title": "Blood Money",
        "hadeeths_count": "12",
        "parent_id": "127"
    },
    {
        "id": "221",
        "title": "Rulings of Prescribed Punishments",
        "hadeeths_count": "3",
        "parent_id": "128"
    },
    {
        "id": "223",
        "title": "Conditions of implementing Prescribed Punishments",
        "hadeeths_count": "5",
        "parent_id": "128"
    },
    {
        "id": "224",
        "title": "Prescribed Punishment for Adultery",
        "hadeeths_count": "11",
        "parent_id": "128"
    },
    {
        "id": "225",
        "title": "Prescribed Punishment for Calumny",
        "hadeeths_count": "4",
        "parent_id": "128"
    },
    {
        "id": "226",
        "title": "Prescribed Punishment for Drinking Alcohol",
        "hadeeths_count": "7",
        "parent_id": "128"
    },
    {
        "id": "227",
        "title": "Prescribed Punishment for Theft",
        "hadeeths_count": "11",
        "parent_id": "128"
    },
    {
        "id": "228",
        "title": "Prescribed Punishment for Highway Robbery",
        "hadeeths_count": "2",
        "parent_id": "128"
    },
    {
        "id": "229",
        "title": "Prescribed Punishment for Rebles (Transgressors)",
        "hadeeths_count": "1",
        "parent_id": "128"
    },
    {
        "id": "230",
        "title": "Prescribed Punishment for Apostasy",
        "hadeeths_count": "2",
        "parent_id": "128"
    },
    {
        "id": "231",
        "title": "Rulings of Discretionary Punishments",
        "hadeeths_count": "2",
        "parent_id": "128"
    },
    {
        "id": "232",
        "title": "Judiciary: Its Ruling, Merit, and Significance",
        "hadeeths_count": "1",
        "parent_id": "129"
    },
    {
        "id": "233",
        "title": "Manners of Judges",
        "hadeeths_count": "2",
        "parent_id": "129"
    },
    {
        "id": "234",
        "title": "Method of Judgment",
        "hadeeths_count": "2",
        "parent_id": "129"
    },
    {
        "id": "235",
        "title": "Claims and Proofs",
        "hadeeths_count": "10",
        "parent_id": "129"
    },
    {
        "id": "236",
        "title": "Testimonies",
        "hadeeths_count": "4",
        "parent_id": "129"
    },
    {
        "id": "249",
        "title": "Shariah Ruling",
        "hadeeths_count": "3",
        "parent_id": "132"
    },
    {
        "id": "250",
        "title": "Juristic and Usooli (Juristic Priciples) Rules",
        "hadeeths_count": "1",
        "parent_id": "132"
    },
    {
        "id": "253",
        "title": "The Book (the Qur'an)",
        "hadeeths_count": "1",
        "parent_id": "132"
    },
    {
        "id": "258",
        "title": "Abrogation",
        "hadeeths_count": "2",
        "parent_id": "132"
    },
    {
        "id": "259",
        "title": "Significations and Inference",
        "hadeeths_count": "3",
        "parent_id": "132"
    },
    {
        "id": "260",
        "title": "Personal Reasoning and Imitation",
        "hadeeths_count": "1",
        "parent_id": "132"
    },
    {
        "id": "261",
        "title": "Divergence and Preponderance",
        "hadeeths_count": "1",
        "parent_id": "132"
    },
    {
        "id": "262",
        "title": "Shariah Objectives",
        "hadeeths_count": "2",
        "parent_id": "132"
    },
    {
        "id": "265",
        "title": "Virtues",
        "hadeeths_count": "149",
        "parent_id": "5"
    },
    {
        "id": "266",
        "title": "Jurisprudence of Ethics",
        "hadeeths_count": "131",
        "parent_id": "5"
    },
    {
        "id": "267",
        "title": "Shariah-approved Manners",
        "hadeeths_count": "201",
        "parent_id": "5"
    },
    {
        "id": "268",
        "title": "Jurisprudence of Supplications and Remembrance of Allah",
        "hadeeths_count": "129",
        "parent_id": "5"
    },
    {
        "id": "269",
        "title": "Heart-Softeners and Sermons",
        "hadeeths_count": "179",
        "parent_id": "5"
    },
    {
        "id": "270",
        "title": "Excellence of Knowledge",
        "hadeeths_count": "10",
        "parent_id": "265"
    },
    {
        "id": "271",
        "title": "Excellence of Monotheism",
        "hadeeths_count": "5",
        "parent_id": "265"
    },
    {
        "id": "272",
        "title": "Merits of the Noble Qur'an",
        "hadeeths_count": "5",
        "parent_id": "265"
    },
    {
        "id": "273",
        "title": "Merits of Being Dutiful to One's Parents",
        "hadeeths_count": "12",
        "parent_id": "265"
    },
    {
        "id": "274",
        "title": "Merits of Maintaining Kinship Ties",
        "hadeeths_count": "2",
        "parent_id": "265"
    },
    {
        "id": "275",
        "title": "Merits of Prophet's Family",
        "hadeeths_count": "9",
        "parent_id": "265"
    },
    {
        "id": "276",
        "title": "Merits of the Companions",
        "hadeeths_count": "34",
        "parent_id": "265"
    },
    {
        "id": "277",
        "title": "Merits of Good Deeds",
        "hadeeths_count": "32",
        "parent_id": "265"
    },
    {
        "id": "278",
        "title": "Merits of Remembering Allah",
        "hadeeths_count": "22",
        "parent_id": "265"
    },
    {
        "id": "279",
        "title": "Merits of Supplication",
        "hadeeths_count": "3",
        "parent_id": "265"
    },
    {
        "id": "280",
        "title": "Merits of Heart Acts",
        "hadeeths_count": "8",
        "parent_id": "265"
    },
    {
        "id": "281",
        "title": "Merits of Organs' Acts",
        "hadeeths_count": "7",
        "parent_id": "265"
    },
    {
        "id": "282",
        "title": "Praiseworthy Morals",
        "hadeeths_count": "79",
        "parent_id": "266"
    },
    {
        "id": "283",
        "title": "Blameworthy Morals",
        "hadeeths_count": "50",
        "parent_id": "266"
    },
    {
        "id": "284",
        "title": "Manners of Scholars and Learners",
        "hadeeths_count": "13",
        "parent_id": "267"
    },
    {
        "id": "285",
        "title": "Manners of Reciting the Noble Qur'an",
        "hadeeths_count": "1",
        "parent_id": "267"
    },
    {
        "id": "286",
        "title": "Manners of Greeting and Seeking Permission",
        "hadeeths_count": "29",
        "parent_id": "267"
    },
    {
        "id": "287",
        "title": "Manners of Speaking and Keeping Silent",
        "hadeeths_count": "31",
        "parent_id": "267"
    },
    {
        "id": "288",
        "title": "Manners of Divergence",
        "hadeeths_count": "3",
        "parent_id": "267"
    },
    {
        "id": "289",
        "title": "Manners of Debate",
        "hadeeths_count": "1",
        "parent_id": "267"
    },
    {
        "id": "290",
        "title": "Manners of Eating and Drinking",
        "hadeeths_count": "39",
        "parent_id": "267"
    },
    {
        "id": "291",
        "title": "Manners of the Road and the Market",
        "hadeeths_count": "4",
        "parent_id": "267"
    },
    {
        "id": "292",
        "title": "Manners and Rulings of Travel",
        "hadeeths_count": "21",
        "parent_id": "267"
    },
    {
        "id": "293",
        "title": "Manners of Sleeping and Waking Up",
        "hadeeths_count": "6",
        "parent_id": "267"
    },
    {
        "id": "294",
        "title": "Manners of Visions",
        "hadeeths_count": "9",
        "parent_id": "267"
    },
    {
        "id": "295",
        "title": "Manners of Visiting and Seeking Permission",
        "hadeeths_count": "13",
        "parent_id": "267"
    },
    {
        "id": "296",
        "title": "Manners of Sneezing and Yawning",
        "hadeeths_count": "6",
        "parent_id": "267"
    },
    {
        "id": "297",
        "title": "Manners of Visiting the Sick",
        "hadeeths_count": "9",
        "parent_id": "267"
    },
    {
        "id": "298",
        "title": "Manners of Dressing",
        "hadeeths_count": "14",
        "parent_id": "267"
    },
    {
        "id": "299",
        "title": "Prophetic Guidance on Remembering Allah",
        "hadeeths_count": "9",
        "parent_id": "268"
    },
    {
        "id": "300",
        "title": "Benefits of Remembering Allah",
        "hadeeths_count": "12",
        "parent_id": "268"
    },
    {
        "id": "301",
        "title": "Morning and Evening Dhikr",
        "hadeeths_count": "7",
        "parent_id": "268"
    },
    {
        "id": "302",
        "title": "Timeless Dhikr",
        "hadeeths_count": "9",
        "parent_id": "268"
    },
    {
        "id": "303",
        "title": "Dhikr on Entering and Leaving the House",
        "hadeeths_count": "2",
        "parent_id": "268"
    },
    {
        "id": "305",
        "title": "Dhikr on Entering and Leaving the Bathroom",
        "hadeeths_count": "1",
        "parent_id": "268"
    },
    {
        "id": "306",
        "title": "Dhikr on Entering and Leaving the Mosque",
        "hadeeths_count": "1",
        "parent_id": "268"
    },
    {
        "id": "307",
        "title": "Hard Times Dhikr",
        "hadeeths_count": "4",
        "parent_id": "268"
    },
    {
        "id": "308",
        "title": "Dhikr on Special Occasions",
        "hadeeths_count": "21",
        "parent_id": "268"
    },
    {
        "id": "309",
        "title": "Rulings of Supplication",
        "hadeeths_count": "3",
        "parent_id": "268"
    },
    {
        "id": "310",
        "title": "Types of Supplication",
        "hadeeths_count": "1",
        "parent_id": "268"
    },
    {
        "id": "311",
        "title": "Manners of Supplication",
        "hadeeths_count": "9",
        "parent_id": "268"
    },
    {
        "id": "312",
        "title": "Causes for Answering or not Answering Supplications",
        "hadeeths_count": "11",
        "parent_id": "268"
    },
    {
        "id": "313",
        "title": "Reported Supplications",
        "hadeeths_count": "39",
        "parent_id": "268"
    },
    {
        "id": "314",
        "title": "Acts of Heart",
        "hadeeths_count": "23",
        "parent_id": "269"
    },
    {
        "id": "315",
        "title": "Heart Diseases",
        "hadeeths_count": "3",
        "parent_id": "269"
    },
    {
        "id": "316",
        "title": "Asceticism and Piety",
        "hadeeths_count": "15",
        "parent_id": "269"
    },
    {
        "id": "317",
        "title": "States of the Righteous Believers",
        "hadeeths_count": "11",
        "parent_id": "269"
    },
    {
        "id": "318",
        "title": "Condemning Sins",
        "hadeeths_count": "17",
        "parent_id": "269"
    },
    {
        "id": "319",
        "title": "Condemning Love of the World",
        "hadeeths_count": "22",
        "parent_id": "269"
    },
    {
        "id": "320",
        "title": "Condemning Whims and Desires",
        "hadeeths_count": "5",
        "parent_id": "269"
    },
    {
        "id": "321",
        "title": "Repentance",
        "hadeeths_count": "12",
        "parent_id": "269"
    },
    {
        "id": "322",
        "title": "Purification of Souls",
        "hadeeths_count": "14",
        "parent_id": "269"
    },
    {
        "id": "323",
        "title": "Terrors of the Graves",
        "hadeeths_count": "3",
        "parent_id": "269"
    },
    {
        "id": "324",
        "title": "Descriptions of Paradise and Hell",
        "hadeeths_count": "52",
        "parent_id": "269"
    },
    {
        "id": "325",
        "title": "Calling to Allah (Da‘wah)",
        "hadeeths_count": "36",
        "parent_id": "6"
    },
    {
        "id": "326",
        "title": "Enjoining Good and Forbidding Evil",
        "hadeeths_count": "11",
        "parent_id": "6"
    },
    {
        "id": "327",
        "title": "Shariah-approved Politics",
        "hadeeths_count": "50",
        "parent_id": "6"
    },
    {
        "id": "328",
        "title": "Islamic Culture",
        "hadeeths_count": "1",
        "parent_id": "6"
    },
    {
        "id": "329",
        "title": "Ruling of Calling to Allah",
        "hadeeths_count": "1",
        "parent_id": "325"
    },
    {
        "id": "331",
        "title": "Manners of Calling to Allah",
        "hadeeths_count": "3",
        "parent_id": "325"
    },
    {
        "id": "334",
        "title": "Backgrounds and Duties of the Callers to Allah",
        "hadeeths_count": "2",
        "parent_id": "325"
    },
    {
        "id": "338",
        "title": "Excellence and Merits of Islam",
        "hadeeths_count": "12",
        "parent_id": "325"
    },
    {
        "id": "339",
        "title": "Universality of Islam",
        "hadeeths_count": "2",
        "parent_id": "325"
    },
    {
        "id": "340",
        "title": "Human Rights in Islam",
        "hadeeths_count": "4",
        "parent_id": "325"
    },
    {
        "id": "341",
        "title": "Animal Rights in Islam",
        "hadeeths_count": "10",
        "parent_id": "325"
    },
    {
        "id": "344",
        "title": "Ruling of Enjoining Good and Forbidding Evil",
        "hadeeths_count": "3",
        "parent_id": "326"
    },
    {
        "id": "345",
        "title": "Excellence of Enjoining Good and Forbidding Evil",
        "hadeeths_count": "3",
        "parent_id": "326"
    },
    {
        "id": "346",
        "title": "Manners of Enjoining Good and Forbidding Evil",
        "hadeeths_count": "1",
        "parent_id": "326"
    },
    {
        "id": "348",
        "title": "Requirements of Enjoining Good and Forbidding Evil",
        "hadeeths_count": "2",
        "parent_id": "326"
    },
    {
        "id": "349",
        "title": "Rulings and Issues of Enjoining Good and Forbidding Evil",
        "hadeeths_count": "2",
        "parent_id": "326"
    },
    {
        "id": "350",
        "title": "Ways of Electing the Supreme Muslim Imam (Ruler)",
        "hadeeths_count": "1",
        "parent_id": "327"
    },
    {
        "id": "351",
        "title": "Requirements of the Supreme Imamate (Leadership)",
        "hadeeths_count": "4",
        "parent_id": "327"
    },
    {
        "id": "352",
        "title": "Duties of the Imam",
        "hadeeths_count": "17",
        "parent_id": "327"
    },
    {
        "id": "353",
        "title": "Imam's Rights over the Subjects",
        "hadeeths_count": "16",
        "parent_id": "327"
    },
    {
        "id": "354",
        "title": "Rebelling against the Muslim Ruler",
        "hadeeths_count": "5",
        "parent_id": "327"
    },
    {
        "id": "355",
        "title": "International Relations in Islam",
        "hadeeths_count": "1",
        "parent_id": "327"
    },
    {
        "id": "356",
        "title": "Consultation System in Islam",
        "hadeeths_count": "1",
        "parent_id": "327"
    },
    {
        "id": "365",
        "title": "Islamic Civilization",
        "hadeeths_count": "1",
        "parent_id": "328"
    },
    {
        "id": "367",
        "title": "Prophet's Biography",
        "hadeeths_count": "205",
        "parent_id": "7"
    },
    {
        "id": "368",
        "title": "History",
        "hadeeths_count": "22",
        "parent_id": "7"
    },
    {
        "id": "392",
        "title": "Prophet's Wives and Family Issues",
        "hadeeths_count": "15",
        "parent_id": "367"
    },
    {
        "id": "393",
        "title": "Prophet's Children",
        "hadeeths_count": "3",
        "parent_id": "367"
    },
    {
        "id": "397",
        "title": "Prophet's Servants",
        "hadeeths_count": "1",
        "parent_id": "367"
    },
    {
        "id": "398",
        "title": "Prophet's Life before Mission",
        "hadeeths_count": "2",
        "parent_id": "367"
    },
    {
        "id": "399",
        "title": "Prophet's Mission",
        "hadeeths_count": "1",
        "parent_id": "367"
    },
    {
        "id": "400",
        "title": "The Makkan Period",
        "hadeeths_count": "5",
        "parent_id": "367"
    },
    {
        "id": "401",
        "title": "The Emigration (Hijrah)",
        "hadeeths_count": "3",
        "parent_id": "367"
    },
    {
        "id": "402",
        "title": "The Madinan Period",
        "hadeeths_count": "1",
        "parent_id": "367"
    },
    {
        "id": "403",
        "title": "Prophet's Battles and Expeditions",
        "hadeeths_count": "30",
        "parent_id": "367"
    },
    {
        "id": "404",
        "title": "Prophet's Correspondences",
        "hadeeths_count": "1",
        "parent_id": "367"
    },
    {
        "id": "405",
        "title": "Prophet's Death",
        "hadeeths_count": "18",
        "parent_id": "367"
    },
    {
        "id": "406",
        "title": "Muhammadan Qualities",
        "hadeeths_count": "106",
        "parent_id": "367"
    },
    {
        "id": "407",
        "title": "Stories and Conditions of Pre-Islamic Nations",
        "hadeeths_count": "11",
        "parent_id": "368"
    },
    {
        "id": "408",
        "title": "History of Makkah, Madinah, and the Aqsa (Jerusalem)",
        "hadeeths_count": "1",
        "parent_id": "368"
    },
    {
        "id": "409",
        "title": "Wars and Battles",
        "hadeeths_count": "3",
        "parent_id": "368"
    },
    {
        "id": "413",
        "title": "Biographies (of Famous Figures)",
        "hadeeths_count": "3",
        "parent_id": "368"
    },
    {
        "id": "414",
        "title": "Countries and Figures",
        "hadeeths_count": "1",
        "parent_id": "368"
    },
    {
        "id": "415",
        "title": "Periodical Occasions",
        "hadeeths_count": "3",
        "parent_id": "368"
    },
    {
        "id": "431",
        "title": "Rulings of Water",
        "hadeeths_count": "6",
        "parent_id": "133"
    },
    {
        "id": "432",
        "title": "Removing Impurities",
        "hadeeths_count": "13",
        "parent_id": "133"
    },
    {
        "id": "434",
        "title": "Utensils",
        "hadeeths_count": "5",
        "parent_id": "133"
    },
    {
        "id": "435",
        "title": "Toilet Manners",
        "hadeeths_count": "20",
        "parent_id": "133"
    },
    {
        "id": "436",
        "title": "Natural Cleanliness Practices",
        "hadeeths_count": "8",
        "parent_id": "133"
    },
    {
        "id": "437",
        "title": "Ablution",
        "hadeeths_count": "39",
        "parent_id": "133"
    },
    {
        "id": "438",
        "title": "Ritual Bath",
        "hadeeths_count": "27",
        "parent_id": "133"
    },
    {
        "id": "439",
        "title": "Dry Ablution",
        "hadeeths_count": "8",
        "parent_id": "133"
    },
    {
        "id": "440",
        "title": "Menses, Postpartum Bleeding, Extra-Menses Bleeding",
        "hadeeths_count": "13",
        "parent_id": "133"
    },
    {
        "id": "441",
        "title": "Excellence of Ablution",
        "hadeeths_count": "4",
        "parent_id": "437"
    },
    {
        "id": "442",
        "title": "Pillars of Ablution",
        "hadeeths_count": "2",
        "parent_id": "437"
    },
    {
        "id": "443",
        "title": "Recommended Acts and Manners of Ablution",
        "hadeeths_count": "9",
        "parent_id": "437"
    },
    {
        "id": "444",
        "title": "Method of Ablution",
        "hadeeths_count": "10",
        "parent_id": "437"
    },
    {
        "id": "445",
        "title": "Nullifiers of Ablution",
        "hadeeths_count": "10",
        "parent_id": "437"
    },
    {
        "id": "448",
        "title": "Causes of Obligatory Ritual Bath",
        "hadeeths_count": "2",
        "parent_id": "438"
    },
    {
        "id": "450",
        "title": "Recommended Manners of the Ritual Bath",
        "hadeeths_count": "2",
        "parent_id": "438"
    },
    {
        "id": "456",
        "title": "Obligation of Prayer and Ruling on Its Abandoner",
        "hadeeths_count": "3",
        "parent_id": "134"
    },
    {
        "id": "457",
        "title": "Virtue of Prayer",
        "hadeeths_count": "13",
        "parent_id": "134"
    },
    {
        "id": "458",
        "title": "The Azan and Iqaamah",
        "hadeeths_count": "22",
        "parent_id": "134"
    },
    {
        "id": "459",
        "title": "Times Not to Pray",
        "hadeeths_count": "10",
        "parent_id": "134"
    },
    {
        "id": "460",
        "title": "Conditions of Prayer",
        "hadeeths_count": "32",
        "parent_id": "134"
    },
    {
        "id": "461",
        "title": "Pillars of Prayer",
        "hadeeths_count": "2",
        "parent_id": "134"
    },
    {
        "id": "463",
        "title": "Recommended Acts of Prayer",
        "hadeeths_count": "18",
        "parent_id": "134"
    },
    {
        "id": "464",
        "title": "Method of Prayer",
        "hadeeths_count": "54",
        "parent_id": "134"
    },
    {
        "id": "465",
        "title": "Dhikr (Invocation) during Prayer",
        "hadeeths_count": "24",
        "parent_id": "134"
    },
    {
        "id": "466",
        "title": "Nullifiers of Prayer",
        "hadeeths_count": "4",
        "parent_id": "134"
    },
    {
        "id": "467",
        "title": "Mistakes during Prayer",
        "hadeeths_count": "11",
        "parent_id": "134"
    },
    {
        "id": "468",
        "title": "Prostration of Forgetfulness, Recitation, Gratitude",
        "hadeeths_count": "21",
        "parent_id": "134"
    },
    {
        "id": "469",
        "title": "Virtue and Rulings of Congregational Prayer",
        "hadeeths_count": "14",
        "parent_id": "134"
    },
    {
        "id": "470",
        "title": "Rulings of the Imam and Followers in Prayer",
        "hadeeths_count": "29",
        "parent_id": "134"
    },
    {
        "id": "471",
        "title": "Prayer of the People with Excuses",
        "hadeeths_count": "9",
        "parent_id": "134"
    },
    {
        "id": "472",
        "title": "Jumu‘ah (Friday) Prayer",
        "hadeeths_count": "14",
        "parent_id": "134"
    },
    {
        "id": "473",
        "title": "Voluntary Prayer",
        "hadeeths_count": "66",
        "parent_id": "134"
    },
    {
        "id": "476",
        "title": "Prayer of Fear",
        "hadeeths_count": "3",
        "parent_id": "134"
    },
    {
        "id": "478",
        "title": "Merit of Jumu‘ah Prayer",
        "hadeeths_count": "2",
        "parent_id": "472"
    },
    {
        "id": "480",
        "title": "Rulings of Jumu‘ah Prayer",
        "hadeeths_count": "1",
        "parent_id": "472"
    },
    {
        "id": "481",
        "title": "Rulings of Jumu‘ah Sermon",
        "hadeeths_count": "2",
        "parent_id": "472"
    },
    {
        "id": "482",
        "title": "Virtue of Voluntary Prayer",
        "hadeeths_count": "2",
        "parent_id": "473"
    },
    {
        "id": "483",
        "title": "Regular Sunnah (Recommended) Prayers",
        "hadeeths_count": "6",
        "parent_id": "473"
    },
    {
        "id": "484",
        "title": "Voluntary Night Prayer (Qiyaam)",
        "hadeeths_count": "35",
        "parent_id": "473"
    },
    {
        "id": "486",
        "title": "Prayer of the Two Eids",
        "hadeeths_count": "2",
        "parent_id": "473"
    },
    {
        "id": "487",
        "title": "Prayer of the Solar and Lunar Eclipse",
        "hadeeths_count": "4",
        "parent_id": "134"
    },
    {
        "id": "488",
        "title": "Rain-Seeking Prayer",
        "hadeeths_count": "2",
        "parent_id": "134"
    },
    {
        "id": "489",
        "title": "Forenoon Prayer",
        "hadeeths_count": "5",
        "parent_id": "473"
    },
    {
        "id": "490",
        "title": "Guidance-Seeking Prayer",
        "hadeeths_count": "1",
        "parent_id": "473"
    },
    {
        "id": "492",
        "title": "Death and Its Rulings",
        "hadeeths_count": "11",
        "parent_id": "135"
    },
    {
        "id": "493",
        "title": "Washing the Dead",
        "hadeeths_count": "2",
        "parent_id": "135"
    },
    {
        "id": "495",
        "title": "Method of Praying over the Dead",
        "hadeeths_count": "9",
        "parent_id": "135"
    },
    {
        "id": "496",
        "title": "Carrying and Burying the Dead",
        "hadeeths_count": "4",
        "parent_id": "135"
    },
    {
        "id": "497",
        "title": "Consolation",
        "hadeeths_count": "3",
        "parent_id": "135"
    },
    {
        "id": "498",
        "title": "Visiting the Graves",
        "hadeeths_count": "4",
        "parent_id": "135"
    },
    {
        "id": "500",
        "title": "Obligation of Zakah and Ruling of Its Abandoning",
        "hadeeths_count": "1",
        "parent_id": "136"
    },
    {
        "id": "503",
        "title": "Rulings and Issues of Zakah",
        "hadeeths_count": "2",
        "parent_id": "136"
    },
    {
        "id": "504",
        "title": "Zakah of Gold and Silver",
        "hadeeths_count": "1",
        "parent_id": "136"
    },
    {
        "id": "505",
        "title": "Zakah of Livestock",
        "hadeeths_count": "2",
        "parent_id": "136"
    },
    {
        "id": "506",
        "title": "Zakah of Land Produce",
        "hadeeths_count": "2",
        "parent_id": "136"
    },
    {
        "id": "509",
        "title": "Zakat-ul-Fitr (Minor-Eid Charity)",
        "hadeeths_count": "3",
        "parent_id": "136"
    },
    {
        "id": "510",
        "title": "Channels of Zakah (People Who Receive Zakah)",
        "hadeeths_count": "2",
        "parent_id": "136"
    },
    {
        "id": "511",
        "title": "Voluntary Charity",
        "hadeeths_count": "26",
        "parent_id": "136"
    },
    {
        "id": "513",
        "title": "Virtue of Fasting",
        "hadeeths_count": "8",
        "parent_id": "137"
    },
    {
        "id": "514",
        "title": "Recommended Acts of Fasting",
        "hadeeths_count": "7",
        "parent_id": "137"
    },
    {
        "id": "515",
        "title": "Sighting the Crescent",
        "hadeeths_count": "1",
        "parent_id": "137"
    },
    {
        "id": "516",
        "title": "Fasting on the Day of Doubt",
        "hadeeths_count": "1",
        "parent_id": "137"
    },
    {
        "id": "517",
        "title": "Fasting Missed Days of Ramadaan",
        "hadeeths_count": "3",
        "parent_id": "137"
    },
    {
        "id": "518",
        "title": "Fasting of People with Excuses",
        "hadeeths_count": "3",
        "parent_id": "137"
    },
    {
        "id": "519",
        "title": "Nullifiers of Fasting",
        "hadeeths_count": "1",
        "parent_id": "137"
    },
    {
        "id": "520",
        "title": "Fasting Obligations",
        "hadeeths_count": "1",
        "parent_id": "137"
    },
    {
        "id": "521",
        "title": "What is Permissible for the Fasting Person",
        "hadeeths_count": "2",
        "parent_id": "137"
    },
    {
        "id": "522",
        "title": "Fasting Prohibitions",
        "hadeeths_count": "4",
        "parent_id": "137"
    },
    {
        "id": "523",
        "title": "What is Disliked for the Fasting Person",
        "hadeeths_count": "1",
        "parent_id": "137"
    },
    {
        "id": "524",
        "title": "Voluntary Fasting",
        "hadeeths_count": "15",
        "parent_id": "137"
    },
    {
        "id": "525",
        "title": "Seclusion for Worship in Ramadaan (I‘tikaaf)",
        "hadeeths_count": "5",
        "parent_id": "137"
    },
    {
        "id": "526",
        "title": "Last Ten Days of Ramadaan",
        "hadeeths_count": "6",
        "parent_id": "137"
    },
    {
        "id": "532",
        "title": "Virtue of Hajj and Umrah",
        "hadeeths_count": "7",
        "parent_id": "138"
    },
    {
        "id": "533",
        "title": "First Ten Days of Dhul Hijjah (Twelfth Lunar Month)",
        "hadeeths_count": "1",
        "parent_id": "138"
    },
    {
        "id": "534",
        "title": "Rulings of Al-Masjid Al-Haraam, the Prophet's Mosque, and the Aqsa Mosque",
        "hadeeths_count": "6",
        "parent_id": "138"
    },
    {
        "id": "536",
        "title": "Rulings of Ihraam (the Ritual State of Consecration)",
        "hadeeths_count": "2",
        "parent_id": "138"
    },
    {
        "id": "537",
        "title": "Prohibitions of Ihraam",
        "hadeeths_count": "6",
        "parent_id": "138"
    },
    {
        "id": "538",
        "title": "Ransom and Hunting Expiation",
        "hadeeths_count": "2",
        "parent_id": "138"
    },
    {
        "id": "539",
        "title": "Types of Rituals (Pilgrimage)",
        "hadeeths_count": "2",
        "parent_id": "138"
    },
    {
        "id": "542",
        "title": "Obligations of ‘Umrah",
        "hadeeths_count": "1",
        "parent_id": "138"
    },
    {
        "id": "544",
        "title": "How to Make Hajj (Pilgrimage)",
        "hadeeths_count": "9",
        "parent_id": "138"
    },
    {
        "id": "545",
        "title": "Pillars of Hajj (Pilgrimage)",
        "hadeeths_count": "1",
        "parent_id": "138"
    },
    {
        "id": "546",
        "title": "Obligations of Hajj (Pilgrimage)",
        "hadeeths_count": "1",
        "parent_id": "138"
    },
    {
        "id": "550",
        "title": "Sacrificial Animals and Expiations",
        "hadeeths_count": "6",
        "parent_id": "138"
    },
    {
        "id": "551",
        "title": "Sacrifice",
        "hadeeths_count": "6",
        "parent_id": "138"
    },
    {
        "id": "554",
        "title": "Rulings and Issues of Hajj and ‘Umrah",
        "hadeeths_count": "16",
        "parent_id": "138"
    },
    {
        "id": "555",
        "title": "Ruling of Jihad",
        "hadeeths_count": "1",
        "parent_id": "139"
    },
    {
        "id": "556",
        "title": "Excellence of Jihad",
        "hadeeths_count": "43",
        "parent_id": "139"
    },
    {
        "id": "557",
        "title": "Categories of Jihad",
        "hadeeths_count": "2",
        "parent_id": "139"
    },
    {
        "id": "558",
        "title": "Rulings and Issues of Jihad",
        "hadeeths_count": "34",
        "parent_id": "139"
    },
    {
        "id": "559",
        "title": "Manners of Jihad",
        "hadeeths_count": "10",
        "parent_id": "139"
    },
    {
        "id": "560",
        "title": "Rulings of Non-Muslims Living in Muslim Country",
        "hadeeths_count": "2",
        "parent_id": "139"
    },
    {
        "id": "561",
        "title": "Rulings of Truce and Security",
        "hadeeths_count": "3",
        "parent_id": "139"
    },
    {
        "id": "564",
        "title": "Forbidden Sales",
        "hadeeths_count": "11",
        "parent_id": "140"
    },
    {
        "id": "566",
        "title": "Oaths",
        "hadeeths_count": "2",
        "parent_id": "169"
    },
    {
        "id": "567",
        "title": "Vows",
        "hadeeths_count": "3",
        "parent_id": "169"
    },
    {
        "id": "570",
        "title": "Excellence of Marriage",
        "hadeeths_count": "1",
        "parent_id": "191"
    },
    {
        "id": "571",
        "title": "Manners of Marriage",
        "hadeeths_count": "7",
        "parent_id": "191"
    },
    {
        "id": "572",
        "title": "Rulings and Conditions of Marriage",
        "hadeeths_count": "5",
        "parent_id": "191"
    },
    {
        "id": "573",
        "title": "Women Unlawful to Marry",
        "hadeeths_count": "4",
        "parent_id": "191"
    },
    {
        "id": "574",
        "title": "Conditions of Marriage",
        "hadeeths_count": "1",
        "parent_id": "191"
    },
    {
        "id": "575",
        "title": "Marriage-Related Defects",
        "hadeeths_count": "4",
        "parent_id": "191"
    },
    {
        "id": "576",
        "title": "Marrying the Disbelievers",
        "hadeeths_count": "5",
        "parent_id": "191"
    },
    {
        "id": "577",
        "title": "Forbidden Marriages",
        "hadeeths_count": "3",
        "parent_id": "191"
    },
    {
        "id": "579",
        "title": "Dowry",
        "hadeeths_count": "11",
        "parent_id": "191"
    },
    {
        "id": "580",
        "title": "Wedding Banquet",
        "hadeeths_count": "6",
        "parent_id": "191"
    },
    {
        "id": "581",
        "title": "Marital Relations",
        "hadeeths_count": "19",
        "parent_id": "191"
    },
    {
        "id": "583",
        "title": "Ruling of Divorce",
        "hadeeths_count": "2",
        "parent_id": "192"
    },
    {
        "id": "584",
        "title": "Words of Divorce",
        "hadeeths_count": "2",
        "parent_id": "192"
    },
    {
        "id": "585",
        "title": "Sunnah Divorce and Innovative Divorce",
        "hadeeths_count": "5",
        "parent_id": "192"
    },
    {
        "id": "586",
        "title": "Revocable and Irrevocable Divorce",
        "hadeeths_count": "3",
        "parent_id": "192"
    },
    {
        "id": "587",
        "title": "Rulings and Issues of Divorce",
        "hadeeths_count": "6",
        "parent_id": "192"
    },
    {
        "id": "588",
        "title": "Rulings of the Waiting Period",
        "hadeeths_count": "1",
        "parent_id": "198"
    },
    {
        "id": "590",
        "title": "The Divorced Woman's Waiting Period",
        "hadeeths_count": "2",
        "parent_id": "198"
    },
    {
        "id": "591",
        "title": "Waiting Period of the Lost Husband's Wife",
        "hadeeths_count": "2",
        "parent_id": "198"
    },
    {
        "id": "593",
        "title": "Ascertaining Non-Pregnancy",
        "hadeeths_count": "1",
        "parent_id": "198"
    },
    {
        "id": "594",
        "title": "Ruling of Breastfeeding",
        "hadeeths_count": "1",
        "parent_id": "199"
    },
    {
        "id": "595",
        "title": "Breastfeeding that Forbids Marriage",
        "hadeeths_count": "1",
        "parent_id": "199"
    },
    {
        "id": "596",
        "title": "Conditions of Breastfeeding",
        "hadeeths_count": "2",
        "parent_id": "199"
    },
    {
        "id": "597",
        "title": "Consequences of Breastfeeding",
        "hadeeths_count": "2",
        "parent_id": "199"
    },
    {
        "id": "603",
        "title": "Hijab for Muslim Women",
        "hadeeths_count": "2",
        "parent_id": "205"
    },
    {
        "id": "604",
        "title": "Intermixing",
        "hadeeths_count": "1",
        "parent_id": "205"
    },
    {
        "id": "605",
        "title": "Polygamy",
        "hadeeths_count": "1",
        "parent_id": "205"
    },
    {
        "id": "607",
        "title": "Men-Women Relationships",
        "hadeeths_count": "7",
        "parent_id": "205"
    },
    {
        "id": "608",
        "title": "Naming the Newborn",
        "hadeeths_count": "2",
        "parent_id": "206"
    },
    {
        "id": "609",
        "title": "Sacrificing for the Newborn",
        "hadeeths_count": "3",
        "parent_id": "206"
    },
    {
        "id": "610",
        "title": "Providing for Children",
        "hadeeths_count": "1",
        "parent_id": "206"
    },
    {
        "id": "611",
        "title": "Raising Children",
        "hadeeths_count": "2",
        "parent_id": "206"
    },
    {
        "id": "612",
        "title": "Rulings of Ruqyah (protective and healing supplications)",
        "hadeeths_count": "1",
        "parent_id": "211"
    },
    {
        "id": "636",
        "title": "Forbidden Utterances and Tongue Evils",
        "hadeeths_count": "9",
        "parent_id": "287"
    },
    {
        "id": "639",
        "title": "Physical Attributes",
        "hadeeths_count": "2",
        "parent_id": "406"
    },
    {
        "id": "640",
        "title": "Prophet's Dress Code",
        "hadeeths_count": "8",
        "parent_id": "406"
    },
    {
        "id": "641",
        "title": "Prophet's Furniture, Stuff, and Arms",
        "hadeeths_count": "1",
        "parent_id": "406"
    },
    {
        "id": "642",
        "title": "Prophet's Food and Drink",
        "hadeeths_count": "8",
        "parent_id": "406"
    },
    {
        "id": "645",
        "title": "Prophet's Travel",
        "hadeeths_count": "2",
        "parent_id": "406"
    },
    {
        "id": "646",
        "title": "Moral Attributes",
        "hadeeths_count": "57",
        "parent_id": "406"
    },
    {
        "id": "647",
        "title": "Prophet's Guidance",
        "hadeeths_count": "26",
        "parent_id": "406"
    },
    {
        "id": "648",
        "title": "Prophet's Generosity",
        "hadeeths_count": "6",
        "parent_id": "646"
    },
    {
        "id": "649",
        "title": "Prophet's Modesty",
        "hadeeths_count": "1",
        "parent_id": "646"
    },
    {
        "id": "650",
        "title": "Prophet's Humility",
        "hadeeths_count": "7",
        "parent_id": "646"
    },
    {
        "id": "651",
        "title": "Prophet's Courage",
        "hadeeths_count": "1",
        "parent_id": "646"
    },
    {
        "id": "652",
        "title": "Prophet's Gentleness",
        "hadeeths_count": "6",
        "parent_id": "646"
    },
    {
        "id": "653",
        "title": "Prophet's Forgiveness",
        "hadeeths_count": "2",
        "parent_id": "646"
    },
    {
        "id": "654",
        "title": "Prophet's Mercy",
        "hadeeths_count": "17",
        "parent_id": "646"
    },
    {
        "id": "655",
        "title": "Prophet's Speech",
        "hadeeths_count": "2",
        "parent_id": "646"
    },
    {
        "id": "656",
        "title": "Prophet's Laughing",
        "hadeeths_count": "1",
        "parent_id": "646"
    },
    {
        "id": "657",
        "title": "Prophet's Crying",
        "hadeeths_count": "1",
        "parent_id": "646"
    },
    {
        "id": "659",
        "title": "Prophet's Compassion",
        "hadeeths_count": "3",
        "parent_id": "646"
    },
    {
        "id": "660",
        "title": "Prophet's Asceticism",
        "hadeeths_count": "2",
        "parent_id": "646"
    },
    {
        "id": "661",
        "title": "Prophet's Justice",
        "hadeeths_count": "2",
        "parent_id": "646"
    },
    {
        "id": "662",
        "title": "Prophet's Forbearance",
        "hadeeths_count": "4",
        "parent_id": "646"
    },
    {
        "id": "666",
        "title": "Prophet's Guidance on Public Speaking",
        "hadeeths_count": "2",
        "parent_id": "647"
    },
    {
        "id": "667",
        "title": "Prophet's Guidance on Purification",
        "hadeeths_count": "3",
        "parent_id": "647"
    },
    {
        "id": "668",
        "title": "Prophet's Guidance on Prayer",
        "hadeeths_count": "12",
        "parent_id": "647"
    },
    {
        "id": "669",
        "title": "Prophet's Guidance on Fasting",
        "hadeeths_count": "2",
        "parent_id": "647"
    },
    {
        "id": "671",
        "title": "Prophet's Guidance on Funerals",
        "hadeeths_count": "1",
        "parent_id": "647"
    },
    {
        "id": "678",
        "title": "Prophet's Guidance on Marriage and Treating One's Wife",
        "hadeeths_count": "3",
        "parent_id": "647"
    },
    {
        "id": "679",
        "title": "The Battle of Yamaamah",
        "hadeeths_count": "1",
        "parent_id": "409"
    },
    {
        "id": "721",
        "title": "Rulings and Manners of Eid",
        "hadeeths_count": "1",
        "parent_id": "415"
    },
    {
        "id": "725",
        "title": "The rulings of mosques",
        "hadeeths_count": "28",
        "parent_id": "134"
    },
    {
        "id": "726",
        "title": "Ramadan",
        "hadeeths_count": "1",
        "parent_id": "137"
    },
    {
        "id": "727",
        "title": "Wiping over leather socks and the like",
        "hadeeths_count": "12",
        "parent_id": "133"
    },
    {
        "id": "735",
        "title": "Prophetic characteristics",
        "hadeeths_count": "19",
        "parent_id": "367"
    },
    {
        "id": "738",
        "title": "Interpretation of verses",
        "hadeeths_count": "3",
        "parent_id": "10"
    }
]
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: /categories/roots/?language={language_code}
https://hadeethenc.com/api/v1/categories/roots/?language=en

List root categories by language code.

This endpoint returns root categories (main categories) in specific language, it accepts language iso code and returns json array of objects each object represents a root category.
### Method: GET
>```
>https://hadeethenc.com/api/v1/categories/roots/?language=en
>```
### Query Params

|Param|value|
|---|---|
|language|en|


### Response: 200
```json
[
    {
        "id": "1",
        "title": "The Noble Qur'an and Qur'anic Sciences",
        "hadeeths_count": "59",
        "parent_id": null
    },
    {
        "id": "2",
        "title": "The Hadith and Hadith Sciences",
        "hadeeths_count": "5",
        "parent_id": null
    },
    {
        "id": "3",
        "title": "The Creed",
        "hadeeths_count": "441",
        "parent_id": null
    },
    {
        "id": "4",
        "title": "Jurisprudence and Juristic Principles",
        "hadeeths_count": "1347",
        "parent_id": null
    },
    {
        "id": "5",
        "title": "Virtues and Manners",
        "hadeeths_count": "822",
        "parent_id": null
    },
    {
        "id": "6",
        "title": "Da‘wah and Hisbah",
        "hadeeths_count": "98",
        "parent_id": null
    },
    {
        "id": "7",
        "title": "Seerah and History",
        "hadeeths_count": "228",
        "parent_id": null
    }
]
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: /hadeeths/list/?language={language_code}&category_id={category_id}
https://hadeethenc.com/api/v1/hadeeths/list/?language=en&category_id=1&page=1&per_page=20

List Hadeeths by category id and language iso code.

This endpoint accepts language iso code, category id (both required) and page (represents page number, optional defaults to 1) and per_page (optional defaults to 20) and returns json object containing "data" object which contains array of json objects each object represents a Hadeeth basic information (id, title, translations iso codes), the second object is "meta" containing meta data required for pagination.
### Method: GET
>```
>https://hadeethenc.com/api/v1/hadeeths/list/?language=en&category_id=1&page=1&per_page=20
>```
### Query Params

|Param|value|
|---|---|
|language|en|
|category_id|1|
|page|1|
|per_page|20|


### Response: 200
```json
{
    "data": [
        {
            "id": "1751",
            "title": "The Messenger of Allah (may Allah's peace and blessings be upon him) entered upon us after his daughter had died and said: \"Wash her three times, or five times or more if you find that necessary. Wash her with water and Sidr (ground lotus leaves), add camphor (or a pinch of camphor) to water in the last time, and let me know when you finish.\"",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "vi",
                "ug",
                "ha"
            ]
        },
        {
            "id": "2750",
            "title": "I was taken to perform pilgrimage with the Messenger of Allah (may Allah’s peace and blessings be upon him) in the Farewell Pilgrimage, when I was seven years old.",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "vi",
                "si",
                "ha"
            ]
        },
        {
            "id": "2751",
            "title": "The Messenger of Allah (may Allah’s peace and blessings be upon him) performed Hajj on the back of a camel, and the same mount was carrying his baggage as well.",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "vi",
                "si",
                "ha"
            ]
        },
        {
            "id": "2752",
            "title": "Observing Ribāt (guarding the Muslim frontiers in the cause of Allah) for a day and a night is better than fasting and standing for night prayer for a whole month. If a person dies (while performing Ribāt), he will receive the reward for his righteous deeds perpetually, will receive his provision, and will be saved from the trials of the grave",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "vi",
                "ha"
            ]
        },
        {
            "id": "2753",
            "title": "‘Umrah in Ramadan is equivalent to Hajj – or Hajj with me.",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "vi",
                "ug",
                "ha"
            ]
        },
        {
            "id": "2754",
            "title": "The Prophet (may Allah's peace and blessings be upon him) used to observe I‘tikāf [spiritual retirement in the mosque] during each Ramadan for ten days. The year in which he died, he observed I‘tikāf for twenty days.",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "ug",
                "ha"
            ]
        },
        {
            "id": "2755",
            "title": "‘Ukkāzh, Mijannah, and Dhū al-Majāz were markets in the pre-Islamic period of ignorance. They considered it a sin to trade during the seasons. So it was revealed: {There is no blame upon you for seeking bounty from your Lord.}",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "vi",
                "si",
                "ug",
                "ha"
            ]
        },
        {
            "id": "2756",
            "title": "The actions of every dead person come to a halt except the one who is garrisoned on the frontier in the way of Allah. His deeds will keep growing till the Day of Judgment, and he will be secure from the trial in the grave.",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "ug",
                "ha"
            ]
        },
        {
            "id": "2758",
            "title": "Whoever performs Hajj and does not commit obscenity or commit any evil therein will go back (free of sin) as on the day his mother gave birth to him.",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tr",
                "ur",
                "zh",
                "hi",
                "ug",
                "ku",
                "ha"
            ]
        },
        {
            "id": "2759",
            "title": "The best Jihad for you (women) is an accepted Hajj.",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "vi",
                "ug",
                "ha"
            ]
        },
        {
            "id": "2932",
            "title": "O ‘Abbās, O uncle of the Messenger of Allah, ask Allah for safety in this life and the Hereafter.",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "ha"
            ]
        },
        {
            "id": "2933",
            "title": "A Muslim man went to the Prophet (may Allah's peace and blessings be upon him) while he was in the mosque and called him, saying: \"O Messenger of Allah, I have committed adultery.\"",
            "translations": [
                "ar",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tr",
                "ur",
                "zh",
                "hi",
                "ug",
                "ha"
            ]
        },
        {
            "id": "2934",
            "title": "The Prophet (may Allah's peace and blessings be upon him) arranged for a horse race among the horses that had been especially prepared for that purpose to take place between Al-Hafyā' and Thaniyyat al-Wadā‘.",
            "translations": [
                "ar",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tr",
                "ur",
                "zh",
                "hi",
                "ug",
                "ha"
            ]
        },
        {
            "id": "2935",
            "title": "When anyone of you eats food, let him not wipe his hand until he licks it or has it licked.",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "ug",
                "ha"
            ]
        },
        {
            "id": "2936",
            "title": "When Allah, the Almighty, gathers together (on the Day of Judgment) all the earlier and later generations of mankind, a banner will be raised for every betrayer, and it will be said: \"This is the betrayal of so-and-so, the son of so-and-so.\"",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "vi",
                "ug",
                "ha"
            ]
        },
        {
            "id": "2937",
            "title": "‘Umar ibn al-Khattāb (may Allah be pleased with him) consulted the people about a woman who was caused to miscarry.",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "ha"
            ]
        },
        {
            "id": "2938",
            "title": "Sa‘d ibn ‘Ubādah sought a ruling from the Messenger of Allah (may Allah's peace and blessings be upon him) concerning a vow that was due upon his mother, who had died before she fulfilled it. The Messenger of Allah (may Allah's peace and blessings be upon him) said: \"Fulfill it on her behalf.\"",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "vi",
                "ug",
                "ha"
            ]
        },
        {
            "id": "2939",
            "title": "A spy from among the polytheists came to the Prophet (may Allah's peace and blessings be upon him) while he was on a journey.",
            "translations": [
                "ar",
                "bn",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tl",
                "tr",
                "ur",
                "zh",
                "hi",
                "ha"
            ]
        },
        {
            "id": "2940",
            "title": "Two women from the Hudhayl tribe fought each other. One of them threw a stone at the other, killing her along with what was in her womb.",
            "translations": [
                "ar",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "tr",
                "ur",
                "zh",
                "hi",
                "tl",
                "ug",
                "ha"
            ]
        },
        {
            "id": "2941",
            "title": "Shall I inform you of the gravest of the major sins?",
            "translations": [
                "ar",
                "bs",
                "en",
                "es",
                "fa",
                "fr",
                "id",
                "ru",
                "tr",
                "ur",
                "zh",
                "hi",
                "bn",
                "ku",
                "ha"
            ]
        }
    ],
    "meta": {
        "current_page": "1",
        "last_page": 108,
        "total_items": 2152,
        "per_page": "20"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: /hadeeths/one/?id={hadeeth_id}&language={language_code}
https://hadeethenc.com/api/v1/hadeeths/one/?language=ar&id=2962

https://hadeethenc.com/api/v1/hadeeths/one/?language=en&id=2962

Get single Hadeeth details by Hadeeth id and language iso code.

The response differs when the language is "Arabic" or not, if it's Arabic then it returns all Hadeeth data (id, title, Hadeeth text (matn), explanation, hints (fawaed), word meaning and references), if non Arabic it returns translated parts (id, title, Hadeeth text (matn), explanation and hints (if translated), it doesnt return reference nor word meaning as they are not translated.
### Method: GET
>```
>https://hadeethenc.com/api/v1/hadeeths/one/?language=en&id=2962
>```
### Query Params

|Param|value|
|---|---|
|language|en|
|id|2962|


### Response: 200
```json
{
    "id": "2962",
    "title": "أَوَّلُ مَا يُقْضَى بَيْنَ النَّاسِ يَوْمَ الْقِيَامَةِ فِي الدِّمَاءِ",
    "hadeeth": "عن عبد الله بن مَسعود -رضي الله عنه- قَالَ: قَالَ رَسُولُ اللَّهِ -صلى الله عليه وسلم-: «أَوَّلُ مَا يُقْضَى بَيْنَ النَّاسِ يَوْمَ الْقِيَامَةِ فِي الدِّمَاءِ».",
    "attribution": "متفق عليه، واللفظ لمسلم.",
    "grade": "صحيح.",
    "explanation": "يُحَاسِبُ الله -تعالى- الْخَلَائِقَ يوم القيامة، ثُمَّ يَقْضِى بينهم بعدله، ويبدأ من المظالم  بالْأَهم، وبما أَنَّ الدِّمَاء هي أَعْظم وأَهَمُّ ما يكون من المظَالمِ فِإِنَّهَا أَوْلُ مَا يُقْضَى بِهِ منها في ذلك اليومِ العظيمِ، وهذا فيما بين العباد في المظالم، أما أعمال العبد فأول ما ينظر فيه الصلاة.",
    "hints": [
        "عِظَمُ أَمْرِ الدِّمَاءِ فِإِنَّ الْبَدَاءَةَ تكون بالْأَهمِّ.",
        "إِثبات يوم القيامة والقضاء فيه.",
        "هذا الحديث لا يعارض حديث \"أَوَّلُ مَا يُحَاسَبُ عَنْهُ الْعَبْدُ صَلَاتُهُ\"؛ لَأَنَّ هَذَا بَيْنَ الْعَبْدِ وَرَبِّهِ وَحديث الباب متعلقٌ بما بين الْعبد وبين النَّاسِ، لأن حقوق العباد مبنية على عدم المسامحة.",
        "على المحاكم العناية بأمر الدّماء وأن تجعل له الأولوية."
    ],
    "categories": [
        "85",
        "219"
    ],
    "translations": [
        "ar",
        "bn",
        "bs",
        "en",
        "es",
        "fa",
        "fr",
        "id",
        "ru",
        "tl",
        "tr",
        "ur",
        "zh",
        "hi",
        "ug",
        "ha",
        "pt",
        "ku",
        "ml",
        "sw"
    ],
    "words_meanings": [
        {
            "word": "يُقْضَى ",
            "meaning": " يُحْكَمُ."
        },
        {
            "word": "في الدِّمَاءِ ",
            "meaning": " في القتل وَإِزْهَاقُ الْأَرْوَاح والجروح."
        }
    ],
    "reference": "خلاصة الكلام شرح عمدة الأحكام، لفيصل آل مبارك، ط2، 1412هـ.\nعمدة الأحكام من كلام خير الأنام صلى الله عليه وسلم، لعبد الغني المقدسي، دراسة وتحقيق: محمود الأرناؤوط، مراجعة وتقديم: عبد القادر الأرناؤوط، ط2، دار الثقافة العربية، دمشق ، بيروت، مؤسسة قرطبة، 1408 هـ.\nصحيح البخاري، تحقيق: محمد زهير بن ناصر الناصر، ط1، دار طوق النجاة (مصورة عن السلطانية بإضافة ترقيم: محمد فؤاد عبد الباقي)، 1422هـ.\nصحيح مسلم، تحقيق: محمد فؤاد عبد الباقي، دار إحياء التراث العربي، بيروت، 1423هـ.\nتأسيس الأحكام للنجمي، ط2، دار علماء السلف، 1414هـ.\nتيسير العلام شرح عمدة الأحكام، للبسام، حققه وعلق عليه وخرج أحاديثه وصنع فهارسه: محمد صبحي بن حسن حلاق، ط10، مكتبة الصحابة، الإمارات، مكتبة التابعين، القاهرة، 1426هـ."
}
```




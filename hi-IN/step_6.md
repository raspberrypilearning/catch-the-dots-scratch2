## कठिनाई बढ़ाना

चलिए बिंदु दिखाई देने के अन्तराल को धीरे-धीरे कम करके, अधिक समय तक जीवित रहने वाले खिलाड़ी के लिए कठिनाई पैदा की जाए।



+ `देरी`{:class="blockdata"} नामक नया वेरिएबल बनाएँ।

+ अपनी स्टेज पर, नई स्क्रिप्ट बनाएं, जो अधिक अन्तराल सेट करती है, और फिर इसे धीरे-धीरे कम करती है।

	```blocks
		जब ⚑ क्लिक किया गया हो
		[delay v] पर (8) सेट करे
		<(delay) = (2)> तक दोहराते रहे
end
			(10) सेकेंड तक ठहरे
			[delay v] से (-0.5) बदले
		end
	```

	ध्यान दें कि यह इसके बहुत समान है जैसे गेम टाइमर काम करता है!

+ अंततः, आप अपने लाल, पीले और नीले बिन्दुओं की स्क्रिप्ट में इस `देरी`{:class="blockdata"} वेरिएबल का उपयोग कर सकते हैं। क्लोन बनाने और अपने नए `देरी`{:class="blockdata"} वेरिएबल से प्रतिस्थापित करने के लिए यादृच्छिक संख्या में सेकंड की प्रतीक्षा करने वाले कोड को हटाएँ।

	```blocks
		(delay) सेकेंड तक ठहरे
	```

+ अपने नए `देरी`{:class="blockdata"} वेरिएबल का परीक्षण करें, और देखें कि बिन्दुओं के बीच अन्तराल धीरे-धीरे कम होता है या नहीं। क्या यह सभी 3 रंगीन बिन्दुओं के लिए काम करता है? क्या आप `देरी`{:class="blockdata"} वेरिएबल का मान कम होते देख सकते हैं?




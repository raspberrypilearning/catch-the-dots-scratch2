## أعلى نتيجة

لنقم بحفظ أعلى نتيجة، ليعرف اللاعب أداءه.



+ أنشئ متغيرًا جديدًا يُسمى `أعلى نتيجة`{:class="blockdata"}.

+ انقر فوق المنصة، وأنشئ قالب مخصص يُسمى `ابحث عن أعلى نتيجة`{:class="blockmoreblocks"}.

	![screenshot](images/dots-custom-1.png)

+ قبل نهاية اللعبة مباشرة، أضف القالب المخصص.

	![screenshot](images/dots-custom-2.png)

+ أضف تعليمة برمجية إلى القالب المخصص لتخزين قيمة `النتيجة`{:class="blockdata"} الحالية على أنها `أعلى نتيجة`{:class="blockdata"} `if`{:class="blockcontrol"} كانت هي أعلى نتيجة حتى انتهاء اللعبة:

	```blocks
		تعريف (check high score)
    إذا <(score) > (high score)> 
      اجعل [high score v] مساوياً (score)
    end
	```

+ اختبر التعليمة البرمجية التي أضفتها. العب اللعبة للتحقق من تحديث `أعلى نتيجة`{:class="blockdata"} بشكل صحيح.




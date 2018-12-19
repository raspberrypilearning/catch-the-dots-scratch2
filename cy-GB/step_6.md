## Gwneud y gêm yn anoddach

Fe wnawn ni wneud y gêm i fynd yn anoddach yr hirach mae'r chwareuwr yn chwarae, gan leihau yr amser rhwng bod pob dot yn ymddangos.

+ Bydd angen creu newidyn newydd o'r enw `oedi`{:class="blockdata"}.

+ Ar dy lwyfan, bydd angen creu sgript newydd sydd yn gosod yr oedi i rif uchel, ac yna yn lleihau yr amser oedi yn araf.

	```blocks
		pan fo ⚑ wedi ei glicio
			gosod [oedi v] i (8)
			ailwna hyd at <(oedi) = (2)>
   		aros (10) eiliad
   		newid [oedi v] gan (-0.5)
		end
	```

	Sylwa fod hyn yn debyg iawn i sut mae'r amserydd gêm yn gweithio!

+ Fe alli di ddefnyddio'r newidyn `oedi`{:class="blockdata"} ar gyfer sgriptiau'r dotiau coch, melyn a glas.  Bydd angen cael gwared o'r côd sydd yn aros nifer o eiliadau rhwng creu cloniau, a'i ail-osod gyda'r newidyn `oedi`{:class="blockdata"}:

	```blocks
		aros (oedi) eiliad
	```

+ Profa dy newidyn `oedi`{:class="blockdata"} newydd, a gweld os yw'r oedi rhwng y dotiau yn lleihau yn araf. Ydy hyn yn gweithio ar gyfer y 3 lliw? Wyt ti'n gallu gweld gwerth y newidyn `oedi`{:class="blockdata"} yn lleihau?



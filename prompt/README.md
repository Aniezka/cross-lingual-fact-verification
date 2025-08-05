
In this folder, we present the prompt that was used during the experiments.

```
 messages = [

            {
                "role": "system",

                "content": """Your task is to evaluate the given claim and evidence, then provide a verdict using one of the following labels: false (completely incorrect), true (completely correct), mostly true (mainly correct with minor issues), mostly false (mainly incorrect with minor true elements), partly true/misleading (mix of true and false elements), complicated/hard to categorise (cannot be verified with given evidence) or other (doesn't fit other categories).
                """
            },

            {
                "role": "user",
                "content": """Claim: In Ungheria le tasse sulle imprese sono al 9 per cento e sulle persone fisiche al 15 per cento, e l’Ungheria cresce del 5 per cento.\nEvidence: L'Ungheria, insieme ad altri paesi della Ue (Lussemburgo, Belgio, Olanda, ... Puntando su una tassazione dei redditi di forte vantaggio (9% per le società e 15% per le ... Per bilanciare la bassa imposizione fiscale su imprese e persone fisiche, ... L'Iva è generalmente al 27% anche se esistono aliquote al 18% e al 5%.
                """
            },

            {
                "role": "assistant",

                "content": """Label: true
                """
            },

            {
                "role": "user",
                "content": """Claim: Das Coronavirus enthält HIV-Anteile, wurde also im Labor erschaffen.\nEvidence: Apr 26, 2020 — Paris – Es klingt wie eine wilde Verschwörungstheorie – und doch hat es der französische Virologe Luc Montagnier bei einer Fernsehdisk. Das Coronavirus enthält HIV-Anteile, wurde also im Labor erschaffen. Feb 6, 2020 — Im Internet kursieren wilde Theorien über den Ursprung des Virus. Dazu tragen auch fragwürdige „Forscher“ bei. Schnelle Studien enthalten oft ...
                """
            },

            {
                "role": "assistant",

                "content": """Label: false
                """
            },

            {
                "role": "user",
                "content": """Claim: “La velocidad promedio de Internet en 2015 era apenas de 4,5 megabits por segundo, hoy la triplicamos”.\nEvidence: Mar 5, 2019 — Macri: “La velocidad promedio de Internet en 2015 era apenas de 4,5 megabits por segundo, hoy la triplicamos”. ¿Es así? Leé el chequeo acá: ...
                """
            },

            {
                "role": "assistant",

                "content": """Label: mostly true
                """
            },

            {
                "role": "user",
                "content": """Claim: „Trenutno se radi na popisu državne imovine..\nEvidence: Državna imovina u RH klasificira se, evidentira i vrednuje na neodgovarajući način. • Glavna knjiga Državne riznice ne ... prosinca svake godine provesti sveobuhvatni popis državne imovine kojom ... rad na izradi aplikacijskog rješenja za drugu fazu ISUDIO je u tijeku. (dovršenje se ... trenutno važećem Zakonu):. Poseban ...
                """
            },

            {
                "role": "assistant",

                "content": """Label: mostly false
                """
            },

            {
                "role": "user",
                "content": """Claim: "ევროპული ღირებულებები" - იტალიის სამაშველო სამსახურებს მიგრანტების ჩაძირული გემების დახმარება აეკრძ...\nEvidence: Oct 4, 2018 — იტალიის სამაშველო სამსახურებს მიგრანტების ჩაძირული გემების დახმარება ულტრა-მემარჯვენე შინაგან საქმეთა ...
                """
            },

            {
                "role": "assistant",

                "content": """Label: partly true/misleading
                """
            },
            {
                "role": "user",
                "content": """Claim: A evasão do Pronatec foi de 80%.\nEvidence: Palavras-Chave: Políticas públicas; Avaliação; Implementação; Pronatec ... os cursos FIC foi de 618, o que corresponde a 80,26 % do total de vagas ofertadas. ... Outra questão apontada como causa da evasão, foi a dificuldade, por boa parte ...
                """
            },

            {
                "role": "assistant",

                "content": """Label: complicated/hard to categorise
                """
            },

            {
                "role": "user",
                "content": """ Claim: Yoris Raweyai Bantah Terkait Tuntutan Pembubaran Banser.\nEvidence: Aug 25, 2019 — Anggota DPD terpilih Yorrys Raweyai menyebut hanya menerima selebaran tujuh poin tuntutan warga di Sorong, yang salah satunya meminta ...
                """
            },

            {
                "role": "assistant",

                "content": """Label: other
                """
            },
            {
                "role": "user",
                "content": text,
            },

            {
                "role": "assistant",

                "content": """Label:
                """
            }
    ]
```

# Metrics 

Read in "Data Mining Concepts and Techniques" p.364-370

<img align="right" src="doc/subpagelist.png">
באותה תיקייה בה נמצא תרגיל זה יש קובץ csv בשם “CANCER_TABLE”. בקובץ זה יש 1000 רשומות. כל רשומה מייצגת ביופסיה שנלקחה מנבדקת. העמודה הראשונה בטבלה מייצגת את הקוטר של הביופסיה בס"מ, והעמודה השנייה מייצגת האם הנבדקת חלתה בסרטן בתקופה של עד שנה לאחר מועד ביצוע הביופסיה.

חברת "פלא-סיינס" הציע מודל שלטענתה עובד נפלא: "אם קוטר הגידול מעל 7 ס"מ אז הנבדק יחלה בסרטן בשנה הקרובה ואחרת לא".
בתרגיל זה ננתח ביצועי מודל זה.

חשב והצג confusion matrix עבור המודל.
חשב FP, TP, FN, TN. 
מה המשמעות העסקית של מדדים אלו עבור בעיה זו (נסח אותם בצורה כזו שגם לקוח שאיננו מבין בתחום יוכל להבין את משמעותם)
חשב TPR, FPR עבור המודל וספק משמעות עסקית.
חשב את הדיוק (precision), הכיסוי (recall) והנכונות (accuracy) של המודל.
	
מדד F של מודל הוא הממוצע ההרמוני בין הדיוק והכיסוי שלו. בנוסחה,
F_1=2/(1/recall+1/precision)
הסימון 1 נובע מקיום גרסה ממושקלת F_β של המדד שתלוייה בפרמטר β.
	חשב את מדד F של המודל.

לאחר ניתוח המודל שביצעת, חברת "פלא-סיינס" הציעה שדרוג למודל: במקום מודל מסווג, החברה תספק מודל שידרג את הביופסיות לפי סבירותן לייצג חולה סרטן (בשנה הקרובה). ביופסיה עם דירוג גבוה יותר מייצגת סיכוי גבוה יותר שהיא נלקחה מאדם שיחלה בסרטן בשנה הקרובה.

למה מודל כזה יכול להיות טוב? שווק אותו ללקוח.
שרטט ROC-CURVE	  עבור המודל הנ"ל, ללא שימוש ב- scikit-learn או כל פונקציה מובנית אחרת של פייתון שמחשבת ROC-CURVE ישירות
חשב את ה-AUC. האם המודל טוב מבחינת קריטריון זה? תן משמעות עסקית לגודל שחישבת (שתהיה ברת הבנה ללקוח).
הפוך את מודל הדירוג למודל סיווג באמצעות ה-ROC ששרטטת. הסבר תשובתך.
חשב confusion matrix עבור המודל החדש מסעיף ב'.
חשב TP, FP, TN, FN, TPR, FPR, ACCURACY, PRECISION, RECALL עבור המודל מסעיף ב'.
השווה את המדדים שחישבת בסעיף הקודם למדדים של המודל הראשוני שהוצע על ידי החברה. על איזה מודל היית ממליץ?
חזור על סעיף 7 כאשר אתה עושה שימוש בפונקציות של scikit-learn (או ספריות צד שלישי אחרות) עם כתיבת קוד מינימלי מצידך.

## ನಿಮ್ಮ ರೆಪೊಸಿಟರಿಯಿಂದ ಬ್ರಾಂಚ್ ಅನ್ನು ತೆಗೆದುಹಾಕುವುದು

ನೀವು ಈ ಟ್ಯುಟೋರಿಯಲ್ ಅನ್ನು ಇದುವರೆಗೆ ಅನುಸರಿಸಿದ್ದರೆ, ನಿಮ್ಮ ಬ್ರಾಂಚ್ `<add-seu-nome>` ತನ್ನ ಗುರಿಯನ್ನು ಪೂರ್ಣಗೊಳಿಸಿದೆ, ಮತ್ತು ಅದನ್ನು ನಿಮ್ಮ ಸ್ಥಳೀಯ ರೆಪೊಸಿಟರಿಯಿಂದ ಅಳಿಸುವ ಸಮಯವಾಗಿದೆ. ಇದು ಅಗತ್ಯವಿಲ್ಲ, ಆದರೆ ಆ ಬ್ರಾಂಚ್‌ನ ಹೆಸರೇ ಅದರ ಉದ್ದೇಶವನ್ನು ಸ್ಪಷ್ಟಪಡಿಸುತ್ತದೆ. ಅದರ ಅವಧಿ ಈ ನಿರ್ದಿಷ್ಟತೆಯಿಂದ ಸ್ವಲ್ಪ ಕಾಲ ಮಾತ್ರ ಇರಬಹುದು.

ಮೊದಲು, `<add-seu-nome>` ಬ್ರಾಂಚ್ ಅನ್ನು ನಿಮ್ಮ ಮುಖ್ಯ ಬ್ರಾಂಚ್ (master) ಗೆ ವಿಲೀನಗೊಳಿಸೋಣ, ಆದ್ದರಿಂದ ಅದಕ್ಕೆ ಹೋಗೋಣ:
```
git checkout master
```

`<add-seu-nome>` ಅನ್ನು master ಗೆ ವಿಲೀನಗೊಳಿಸಿ:
```
git merge <add-seu-nome> master
```

`<add-seu-nome>` ಅನ್ನು ನಿಮ್ಮ ಸ್ಥಳೀಯ ರೆಪೊಸಿಟರಿಯಿಂದ ತೆಗೆದುಹಾಕಿ:
```
git branch -d <add-seu-nome>
```

ಈಗ ನೀವು ನಿಮ್ಮ ಸ್ಥಳೀಯ `<add-seu-nome>` ಬ್ರಾಂಚ್ ಅನ್ನು ಅಳಿಸಿದ್ದೀರಿ, ಮತ್ತು ಎಲ್ಲವೂ ಸ್ವಚ್ಛ ಮತ್ತು ಕ್ರಮಬದ್ಧವಾಗಿದೆ.
ಈ ಹಂತದಲ್ಲಿ, ನೀವು ಇನ್ನೂ ನಿಮ್ಮ ಫೋರ್ಕ್‌ನಲ್ಲಿ `<add-seu-nome>` ಬ್ರಾಂಚ್ ಅನ್ನು ಹೊಂದಿರಬಹುದು. ಅದನ್ನು ಅಳಿಸುವ ಮೊದಲು, ನೀವು ಈ ಬ್ರಾಂಚ್‌ನಿಂದ ನನ್ನ ರೆಪೊಸಿಟರಿಗೆ ಪುಲ್ ರಿಕ್ವೆಸ್ಟ್ ಕಳುಹಿಸಿದ್ದೀರಾ ಎಂದು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಿ. ಹೀಗಾಗಿ ನಾನು ಇದನ್ನು ಈಗಾಗಲೇ ವಿಲೀನಗೊಳಿಸಿಲ್ಲದಿದ್ದರೆ, ಅದನ್ನು ಅಳಿಸಬೇಡಿ.

ಆದರೆ, ನಾನು ಈಗಾಗಲೇ ನಿಮ್ಮ ಬ್ರಾಂಚ್ ಅನ್ನು ವಿಲೀನಗೊಳಿಸಿದ್ದರೆ ಮತ್ತು ನೀವು ರಿಮೋಟ್ ಬ್ರಾಂಚ್ ಅನ್ನು ಅಳಿಸಲು ಬಯಸಿದರೆ, ಈ ಆಜ್ಞೆಯನ್ನು ಬಳಸಿ:
```
git push origin --delete <add-seu-nome>
```

ಇತ್ತೀಚಿನ ಬ್ರಾಂಚ್‌ಗಳನ್ನು ನೀವು ಹೇಗೆ ನಿರ್ವಹಿಸಬಹುದು ಎಂಬುದನ್ನು ನೀವು ಈಗ ತಿಳಿದಿದ್ದೀರಿ.
ಕಾಲಾಂತರದಲ್ಲಿ, ನನ್ನ ಸಾರ್ವಜನಿಕ ರೆಪೊಸಿಟರಿಯಲ್ಲಿ ಅನೇಕ ಕಮಿಟ್‌ಗಳು ಸೇರಿಕೊಳ್ಳುತ್ತವೆ. ನಿಮ್ಮ ಲ್ಯಾಪ್‌ಟಾಪ್‌ನಲ್ಲಿನ ಮತ್ತು ಫೋರ್ಕ್‌ನಲ್ಲಿನ ಮುಖ್ಯ ಬ್ರಾಂಚ್‌ಗಳು ಇನ್ನಷ್ಟು ಅಪ್‌ಡೇಟ್ ಆಗಿರುವುದಿಲ್ಲ. ಹೀಗಾಗಿ, ನಿಮ್ಮ ರೆಪೊಸಿಟರಿಗಳನ್ನು ನನ್ನದೊಂದಿಗೆ ಸಿಂಕ್ರೀನೈಸ್ ಮಾಡುವುದಕ್ಕಾಗಿ, ಕೆಳಗಿನ ಹಂತಗಳನ್ನು ಅನುಸರಿಸಿ.

#### [ನಿಮ್ಮ ಫೋರ್ಕ್ ಅನ್ನು ಈ ರೆಪೊಸಿಟರಿಯೊಂದಿಗೆ ಸಿಂಕ್ರೊನೈಸ್ ಮಾಡುವುದು](keeping-your-fork-synced-with-this-repository.pt_br.md)


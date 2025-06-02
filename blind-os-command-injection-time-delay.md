# Blind OS Command Injection with Time Delays

Bu lab-da biz serverdə komanda yerinə yetirilməsini `sleep` funksiyası vasitəsilə **vaxt gecikməsi** ilə yoxlayırıq.

## 🔍 Mərhələlər

1. Burp Suite ilə HTTP sorğunu ələ keçirdim.
2. `message` parametrinin dəyərini aşağıdakı kimi dəyişdim:
$(sleep 10)
3. Sorğunu göndərdim və serverin cavab verməsində 10 saniyəlik gecikmə müşahidə etdim.
4. Bu da göstərdi ki, serverdə **blind OS command injection** mövcuddur.

## 💡 Qeyd

Bu tip zəifliklərdə birbaşa cavab yox olur, amma zaman gecikməsi ilə arxa planda əmrin yerinə yetdiyini təyin edə bilirik.

## 🛠️ İstifadə olunan alətlər

- Burp Suite
- Browser (Chrome)


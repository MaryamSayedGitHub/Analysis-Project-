# 🚴‍♂️ Bike Sharing Data Insights  

This project analyzes bike-sharing trip data to uncover trends related to trip duration, user demographics, and station popularity. Below are key insights and a Q&A section based on the findings.

---

## 📊 Enhancing Insights with Numbers  


### 1️⃣ Quantify Trip Duration Differences  ![download (3)](https://github.com/user-attachments/assets/d8f2fc39-f227-4f8f-8ca6-d9d8b494ceb8)

![download (4)](https://github.com/user-attachments/assets/3d3be32b-97ca-4e2f-9a88-b2cbf6c05e44)

Rather than stating that customers have longer trip durations, provide exact values:  
- **Example:**  
  *"Customers have an average trip duration of **X** minutes, compared to **Y** minutes for subscribers."*  

### 2️⃣ Specify Popular Station Usage  ![download](https://github.com/user-attachments/assets/f0b4c540-72d6-44b1-8f2f-1b086a4b8b34)
Instead of simply listing popular stations, include trip counts:  
- **Example:**  
  *"Market St at 10th St was the most popular start station with **X** trips."*  

### 3️⃣ Provide Age Distribution Statistics  ![download (1)](https://github.com/user-attachments/assets/e0dd11a3-4667-47ad-a60a-2fbfae47c3d2)

Go beyond just the average age and include a more detailed breakdown:  
- **Example:**  
  *"The median user age is **34** years, with **75%** of users between **25 and 45** years old. Approximately **X%** of users fall into the 'Young Adult' category."*  

### 4️⃣ Highlight Correlation Strengths  ![download (2)](https://github.com/user-attachments/assets/9e2a74e5-37f6-4ea1-8ff0-316afdf91b4c)

Use correlation coefficients to measure relationships:  
- **Example:**  
  *"There is a moderate positive correlation (**r = 0.45**) between trip duration and user age."*  

---

## ❓ Q&A Section  

### 🔹 Q1: What is the average trip duration for customers compared to subscribers?  
**A1:** Customers have a significantly longer average trip duration of **X** minutes, compared to **Y** minutes for subscribers.  

### 🔹 Q2: Which start and end stations are the most popular?  
**A2:**  
- The most popular start station is **"Market St at 10th St"** with **X** trips.  
- The most popular end station is **"San Francisco Caltrain Station 2"** with **Y** trips.  

### 🔹 Q3: How is user age distributed across different age groups?  
**A3:**  
- The **median user age** is **34 years**.  
- Most users fall within the **Young Adult** and **Adult** categories, with **X%** in Young Adult and **Y%** in Adult.  

### 🔹 Q4: Is there a relationship between trip duration and user age?  
**A4:** Yes, there is a weak positive correlation (**r = 0.45**) between trip duration and user age, suggesting that older users tend to take slightly longer trips.  

### 🔹 Q5: How does user type influence trip duration?  
**A5:**  
- **Subscribers** tend to have **shorter trips** with an average trip duration of **Y** minutes.  
- **Customers** have **longer trips**, averaging **X** minutes.  [Uploading Untitled21.ipynb<!DOCTYPE html>
<!-- saved from url=(0095)https://colab.research.google.com/drive/1SRMnbgb9yKuwM9M4JRgH7FB5Rigi1Y2g#scrollTo=af5FKJF5mMLV -->
<html lang="en" theme="dark" editor="Default Dark"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8"><meta http-equiv="origin-trial" content="A/kargTFyk8MR5ueravczef/wIlTkbVk1qXQesp39nV+xNECPdLBVeYffxrM8TmZT6RArWGQVCJ0LRivD7glcAUAAACQeyJvcmlnaW4iOiJodHRwczovL2dvb2dsZS5jb206NDQzIiwiZmVhdHVyZSI6IkRpc2FibGVUaGlyZFBhcnR5U3RvcmFnZVBhcnRpdGlvbmluZzIiLCJleHBpcnkiOjE3NDIzNDIzOTksImlzU3ViZG9tYWluIjp0cnVlLCJpc1RoaXJkUGFydHkiOnRydWV9"><meta http-equiv="origin-trial" content="A/kargTFyk8MR5ueravczef/wIlTkbVk1qXQesp39nV+xNECPdLBVeYffxrM8TmZT6RArWGQVCJ0LRivD7glcAUAAACQeyJvcmlnaW4iOiJodHRwczovL2dvb2dsZS5jb206NDQzIiwiZmVhdHVyZSI6IkRpc2FibGVUaGlyZFBhcnR5U3RvcmFnZVBhcnRpdGlvbmluZzIiLCJleHBpcnkiOjE3NDIzNDIzOTksImlzU3ViZG9tYWluIjp0cnVlLCJpc1RoaXJkUGFydHkiOnRydWV9"><script type="text/javascript" async="" charset="utf-8" src="./Untitled21.ipynb - Colab_files/recaptcha__en.js.download" crossorigin="anonymous" integrity="sha384-61VR//KO5vDNAFE1O0P7MzEOKj68zRELxJeYIL5DD4Cj1hdU5Cro7XZfUD04Ca7S" nonce=""></script><script type="text/javascript" async="" charset="utf-8" src="./Untitled21.ipynb - Colab_files/recaptcha__en.js.download" crossorigin="anonymous" integrity="sha384-61VR//KO5vDNAFE1O0P7MzEOKj68zRELxJeYIL5DD4Cj1hdU5Cro7XZfUD04Ca7S" nonce=""></script><script src="./Untitled21.ipynb - Colab_files/cb=gapi.loaded_1" nonce="" async=""></script><script src="./Untitled21.ipynb - Colab_files/cb=gapi.loaded_0" nonce="" async=""></script><script type="text/javascript" async="" src="./Untitled21.ipynb - Colab_files/js" nonce=""></script><script async="" src="./Untitled21.ipynb - Colab_files/analytics.js.download"></script><script nonce="">
      document.addEventListener('keydown', (e) => {
        // Stop propagation on ESC because otherwise it will halt outbound XHRs
        // See b/131755324 for more info.
        if (e.key === 'Escape') {
          e.stopPropagation();
          e.preventDefault();
        }
      });
    </script><meta name="referrer" content="origin"><meta name="viewport" content="width=device-width, initial-scale=1"><title>Untitled21.ipynb - Colab</title><link href="./Untitled21.ipynb - Colab_files/css2" rel="stylesheet"><link href="./Untitled21.ipynb - Colab_files/css" rel="stylesheet"><link rel="search" type="application/opensearchdescription+xml" href="https://colab.research.google.com/opensearch.xml" title="Google Colab"><style>.gb_2d{font:13px/27px Roboto,Arial,sans-serif;z-index:986}@-webkit-keyframes gb__a{0%{opacity:0}50%{opacity:1}}@keyframes gb__a{0%{opacity:0}50%{opacity:1}}a.gb_Qa{border:none;color:#4285f4;cursor:default;font-weight:bold;outline:none;position:relative;text-align:center;text-decoration:none;text-transform:uppercase;white-space:nowrap;-webkit-user-select:none}a.gb_Qa:hover::after,a.gb_Qa:focus::after{background-color:rgba(0,0,0,.12);content:"";height:100%;left:0;position:absolute;top:0;width:100%}a.gb_Qa:hover,a.gb_Qa:focus{text-decoration:none}a.gb_Qa:active{background-color:rgba(153,153,153,.4);text-decoration:none}a.gb_Ra{background-color:#4285f4;color:#fff}a.gb_Ra:active{background-color:#0043b2}.gb_Sa{box-shadow:0 1px 1px rgba(0,0,0,.16)}.gb_Qa,.gb_Ra,.gb_Ta,.gb_Ua{display:inline-block;line-height:28px;padding:0 12px;border-radius:2px}.gb_Ta{background:#f8f8f8;border:1px solid #c6c6c6}.gb_Ua{background:#f8f8f8}.gb_Ta,#gb a.gb_Ta.gb_Ta,.gb_Ua{color:#666;cursor:default;text-decoration:none}#gb a.gb_Ua{cursor:default;text-decoration:none}.gb_Ua{border:1px solid #4285f4;font-weight:bold;outline:none;background:#4285f4;background:-webkit-gradient(linear,left top,left bottom,from(top),color-stop(#4387fd),to(#4683ea));background:-webkit-linear-gradient(top,#4387fd,#4683ea);background:linear-gradient(top,#4387fd,#4683ea);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr=#4387fd,endColorstr=#4683ea,GradientType=0)}#gb a.gb_Ua{color:#fff}.gb_Ua:hover{box-shadow:0 1px 0 rgba(0,0,0,.15)}.gb_Ua:active{box-shadow:inset 0 2px 0 rgba(0,0,0,.15);background:#3c78dc;background:-webkit-gradient(linear,left top,left bottom,from(top),color-stop(#3c7ae4),to(#3f76d3));background:-webkit-linear-gradient(top,#3c7ae4,#3f76d3);background:linear-gradient(top,#3c7ae4,#3f76d3);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr=#3c7ae4,endColorstr=#3f76d3,GradientType=0)}#gb .gb_Va{background:#fff;border:1px solid #dadce0;color:#1a73e8;display:inline-block;text-decoration:none}#gb .gb_Va:hover{background:#f8fbff;border-color:#dadce0;color:#174ea6}#gb .gb_Va:focus{background:#f4f8ff;color:#174ea6;outline:1px solid #174ea6}#gb .gb_Va:active,#gb .gb_Va:focus:active{background:#ecf3fe;color:#174ea6}#gb .gb_Va.gb_H{background:transparent;border:1px solid #5f6368;color:#8ab4f8;text-decoration:none}#gb .gb_Va.gb_H:hover{background:rgba(255,255,255,.04);color:#e8eaed}#gb .gb_Va.gb_H:focus{background:rgba(232,234,237,.12);color:#e8eaed;outline:1px solid #e8eaed}#gb .gb_Va.gb_H:active,#gb .gb_Va.gb_H:focus:active{background:rgba(232,234,237,.1);color:#e8eaed}.gb_cd{display:inline-block;vertical-align:middle}.gb_Ne .gb_Q{bottom:-3px;right:-5px}.gb_D{position:relative}.gb_B{display:inline-block;outline:none;vertical-align:middle;border-radius:2px;box-sizing:border-box;height:40px;width:40px;cursor:pointer;text-decoration:none}#gb#gb a.gb_B{cursor:pointer;text-decoration:none}.gb_B,a.gb_B{color:#000}.gb_dd{border-color:transparent;border-bottom-color:#fff;border-style:dashed dashed solid;border-width:0 8.5px 8.5px;display:none;position:absolute;left:11.5px;top:33px;z-index:1;height:0;width:0;-webkit-animation:gb__a .2s;animation:gb__a .2s}.gb_ed{border-color:transparent;border-style:dashed dashed solid;border-width:0 8.5px 8.5px;display:none;position:absolute;left:11.5px;z-index:1;height:0;width:0;-webkit-animation:gb__a .2s;animation:gb__a .2s;border-bottom-color:rgba(0,0,0,.2);top:32px}x:-o-prefocus,div.gb_ed{border-bottom-color:#ccc}.gb_la{background:#fff;border:1px solid #ccc;border-color:rgba(0,0,0,.2);color:#000;-webkit-box-shadow:0 2px 10px rgba(0,0,0,.2);box-shadow:0 2px 10px rgba(0,0,0,.2);display:none;outline:none;overflow:hidden;position:absolute;right:8px;top:62px;-webkit-animation:gb__a .2s;animation:gb__a .2s;border-radius:2px;-webkit-user-select:text}.gb_cd.gb_Tc .gb_dd,.gb_cd.gb_Tc .gb_ed,.gb_cd.gb_Tc .gb_la,.gb_Tc.gb_la{display:block}.gb_cd.gb_Tc.gb_fd .gb_dd,.gb_cd.gb_Tc.gb_fd .gb_ed{display:none}.gb_Oe{position:absolute;right:8px;top:62px;z-index:-1}.gb_gd .gb_dd,.gb_gd .gb_ed,.gb_gd .gb_la{margin-top:-10px}.gb_cd:first-child,#gbsfw:first-child+.gb_cd{padding-left:4px}.gb_Fa.gb_Pe .gb_cd:first-child{padding-left:0}.gb_Qe{position:relative}.gb_2c .gb_Qe,.gb_Jd .gb_Qe{float:right}.gb_B{padding:8px;cursor:pointer}.gb_B::after{content:"";position:absolute;top:-4px;bottom:-4px;left:-4px;right:-4px}.gb_Fa .gb_hd:not(.gb_Qa):focus img{background-color:rgba(0,0,0,.2);outline:none;-webkit-border-radius:50%;border-radius:50%}.gb_id button svg,.gb_B{-webkit-border-radius:50%;border-radius:50%}.gb_id button:focus:not(:focus-visible) svg,.gb_id button:hover svg,.gb_id button:active svg,.gb_B:focus:not(:focus-visible),.gb_B:hover,.gb_B:active,.gb_B[aria-expanded=true]{outline:none}.gb_Lc .gb_id.gb_jd button:focus-visible svg,.gb_id button:focus-visible svg,.gb_B:focus-visible{outline:1px solid #202124}.gb_Lc .gb_id button:focus-visible svg,.gb_Lc .gb_B:focus-visible{outline:1px solid #f1f3f4}@media (forced-colors:active){.gb_Lc .gb_id.gb_jd button:focus-visible svg,.gb_id button:focus-visible svg,.gb_Lc .gb_id button:focus-visible svg{outline:1px solid currentcolor}}.gb_Lc .gb_id.gb_jd button:focus svg,.gb_Lc .gb_id.gb_jd button:focus:hover svg,.gb_id button:focus svg,.gb_id button:focus:hover svg,.gb_B:focus,.gb_B:focus:hover{background-color:rgba(60,64,67,.1)}.gb_Lc .gb_id.gb_jd button:active svg,.gb_id button:active svg,.gb_B:active{background-color:rgba(60,64,67,.12)}.gb_Lc .gb_id.gb_jd button:hover svg,.gb_id button:hover svg,.gb_B:hover{background-color:rgba(60,64,67,.08)}.gb_Wa .gb_B.gb_Za:hover{background-color:transparent}.gb_B[aria-expanded=true],.gb_B:hover[aria-expanded=true]{background-color:rgba(95,99,104,.24)}.gb_B[aria-expanded=true] .gb_F{fill:#5f6368;opacity:1}.gb_Lc .gb_id button:hover svg,.gb_Lc .gb_B:hover{background-color:rgba(232,234,237,.08)}.gb_Lc .gb_id button:focus svg,.gb_Lc .gb_id button:focus:hover svg,.gb_Lc .gb_B:focus,.gb_Lc .gb_B:focus:hover{background-color:rgba(232,234,237,.1)}.gb_Lc .gb_id button:active svg,.gb_Lc .gb_B:active{background-color:rgba(232,234,237,.12)}.gb_Lc .gb_B[aria-expanded=true],.gb_Lc .gb_B:hover[aria-expanded=true]{background-color:rgba(255,255,255,.12)}.gb_Lc .gb_B[aria-expanded=true] .gb_F{fill:#fff;opacity:1}.gb_cd{padding:4px}.gb_Fa.gb_Pe .gb_cd{padding:4px 2px}.gb_Fa.gb_Pe .gb_z.gb_cd{padding-left:6px}.gb_la{z-index:991;line-height:normal}.gb_la.gb_kd{left:0;right:auto}@media (max-width:350px){.gb_la.gb_kd{left:0}}.gb_Re .gb_la{top:56px}.gb_R{display:none!important}.gb_nd{visibility:hidden}.gb_J .gb_B,.gb_ka .gb_J .gb_B{background-position:-64px -29px}.gb_1 .gb_J .gb_B{background-position:-29px -29px;opacity:1}.gb_J .gb_B,.gb_J .gb_B:hover,.gb_J .gb_B:focus{opacity:1}.gb_L{display:none}@media screen and (max-width:319px){.gb_ld:not(.gb_md) .gb_J{display:none;visibility:hidden}}.gb_Q{display:none}.gb_9c{font-family:Google Sans,Roboto,Helvetica,Arial,sans-serif;font-size:20px;font-weight:400;letter-spacing:0.25px;line-height:48px;margin-bottom:2px;opacity:1;overflow:hidden;padding-left:16px;position:relative;text-overflow:ellipsis;vertical-align:middle;top:2px;white-space:nowrap;-webkit-flex:1 1 auto;-webkit-box-flex:1;flex:1 1 auto}.gb_9c.gb_ad{color:#3c4043}.gb_Fa.gb_cc .gb_9c{margin-bottom:0}.gb_sd.gb_ud .gb_9c{padding-left:4px}.gb_Fa.gb_cc .gb_vd{position:relative;top:-2px}.gb_bd{display:none}.gb_Fa{color:black;min-width:160px;position:relative;-webkit-transition:box-shadow 250ms;transition:box-shadow 250ms}.gb_Fa.gb_Sc{min-width:120px}.gb_Fa.gb_wd .gb_xd{display:none}.gb_Fa.gb_wd .gb_ld{height:56px}header.gb_Fa{display:block}.gb_Fa svg{fill:currentColor}.gb_Dd{position:fixed;top:0;width:100%}.gb_yd{-webkit-box-shadow:0 4px 5px 0 rgba(0,0,0,.14),0 1px 10px 0 rgba(0,0,0,.12),0 2px 4px -1px rgba(0,0,0,.2);box-shadow:0 4px 5px 0 rgba(0,0,0,.14),0 1px 10px 0 rgba(0,0,0,.12),0 2px 4px -1px rgba(0,0,0,.2)}.gb_Ed{height:64px}.gb_ld{-webkit-box-sizing:border-box;box-sizing:border-box;position:relative;width:100%;display:-webkit-box;display:-webkit-flex;display:flex;-webkit-box-pack:space-between;-webkit-justify-content:space-between;justify-content:space-between;min-width:-webkit-min-content;min-width:min-content}.gb_Fa:not(.gb_cc) .gb_ld{padding:8px}.gb_Fa.gb_Fd .gb_ld{-webkit-flex:1 0 auto;-webkit-box-flex:1;flex:1 0 auto}.gb_Fa .gb_ld.gb_md.gb_Hd{min-width:0}.gb_Fa.gb_cc .gb_ld{padding:4px;padding-left:8px;min-width:0}.gb_xd{height:48px;vertical-align:middle;white-space:nowrap;-webkit-box-align:center;-webkit-align-items:center;align-items:center;display:-webkit-box;display:-webkit-flex;display:flex;-webkit-user-select:none}.gb_Ad>.gb_xd{display:table-cell;width:100%}.gb_sd{padding-right:30px;box-sizing:border-box;-webkit-flex:1 0 auto;-webkit-box-flex:1;flex:1 0 auto}.gb_Fa.gb_cc .gb_sd{padding-right:14px}.gb_Bd{-webkit-flex:1 1 100%;-webkit-box-flex:1;flex:1 1 100%}.gb_Bd>:only-child{display:inline-block}.gb_Cd.gb_3c{padding-left:4px}.gb_Cd.gb_Id,.gb_Fa.gb_Fd .gb_Cd,.gb_Fa.gb_cc:not(.gb_Jd) .gb_Cd{padding-left:0}.gb_Fa.gb_cc .gb_Cd.gb_Id{padding-right:0}.gb_Fa.gb_cc .gb_Cd.gb_Id .gb_Wa{margin-left:10px}.gb_3c{display:inline}.gb_Fa.gb_Wc .gb_Cd.gb_Kd,.gb_Fa.gb_Jd .gb_Cd.gb_Kd{padding-left:2px}.gb_9c{display:inline-block}.gb_Cd{-webkit-box-sizing:border-box;box-sizing:border-box;height:48px;line-height:normal;padding:0 4px;padding-left:30px;-webkit-flex:0 0 auto;-webkit-box-flex:0;flex:0 0 auto;-webkit-box-pack:flex-end;-webkit-justify-content:flex-end;justify-content:flex-end}.gb_Jd{height:48px}.gb_Fa.gb_Jd{min-width:auto}.gb_Jd .gb_Cd{float:right;padding-left:32px}.gb_Jd .gb_Cd.gb_Ld{padding-left:0}.gb_Md{font-size:14px;max-width:200px;overflow:hidden;padding:0 12px;text-overflow:ellipsis;white-space:nowrap;-webkit-user-select:text}.gb_pd{-webkit-transition:background-color .4s;-webkit-transition:background-color .4s;transition:background-color .4s}.gb_Nd{color:black}.gb_Lc{color:white}.gb_Fa a,.gb_Pc a{color:inherit}.gb_ba{color:rgba(0,0,0,.87)}.gb_Fa svg,.gb_Pc svg,.gb_sd .gb_td,.gb_2c .gb_td{color:#5f6368;opacity:1}.gb_Lc svg,.gb_Pc.gb_Uc svg,.gb_Lc .gb_sd .gb_td,.gb_Lc .gb_sd .gb_Kc,.gb_Lc .gb_sd .gb_vd,.gb_Pc.gb_Uc .gb_td{color:rgba(255,255,255,.87)}.gb_Lc .gb_sd .gb_Od:not(.gb_Pd){opacity:.87}.gb_ad{color:inherit;opacity:1;text-rendering:optimizeLegibility;-webkit-font-smoothing:antialiased}.gb_Lc .gb_ad,.gb_Nd .gb_ad{opacity:1}.gb_Qd{position:relative}.gb_M{font-family:arial,sans-serif;line-height:normal;padding-right:15px}a.gb_X,span.gb_X{color:rgba(0,0,0,.87);text-decoration:none}.gb_Lc a.gb_X,.gb_Lc span.gb_X{color:white}a.gb_X:focus{outline-offset:2px}a.gb_X:hover{text-decoration:underline}.gb_Z{display:inline-block;padding-left:15px}.gb_Z .gb_X{display:inline-block;line-height:24px;vertical-align:middle}.gb_qd{font-family:Google Sans,Roboto,Helvetica,Arial,sans-serif;font-weight:500;font-size:14px;letter-spacing:.25px;line-height:16px;margin-left:10px;margin-right:8px;min-width:96px;padding:9px 23px;text-align:center;vertical-align:middle;border-radius:4px;box-sizing:border-box}.gb_Fa.gb_Jd .gb_qd{margin-left:8px}#gb a.gb_Ua.gb_qd{cursor:pointer}.gb_Ua.gb_qd:hover{background:#1b66c9;-webkit-box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3);box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3)}.gb_Ua.gb_qd:focus,.gb_Ua.gb_qd:hover:focus{background:#1c5fba;-webkit-box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3);box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3)}.gb_Ua.gb_qd:active{background:#1b63c1;-webkit-box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3);box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3)}.gb_qd{background:#1a73e8;border:1px solid transparent}.gb_Fa.gb_cc .gb_qd{padding:9px 15px;min-width:80px}.gb_Rd{text-align:left}#gb .gb_Lc a.gb_qd:not(.gb_H),#gb.gb_Lc a.gb_qd{background:#fff;border-color:#dadce0;-webkit-box-shadow:none;box-shadow:none;color:#1a73e8}#gb a.gb_Ua.gb_H.gb_qd{background:#8ab4f8;border:1px solid transparent;-webkit-box-shadow:none;box-shadow:none;color:#202124}#gb .gb_Lc a.gb_qd:hover:not(.gb_H),#gb.gb_Lc a.gb_qd:hover{background:#f8fbff;border-color:#cce0fc}#gb a.gb_Ua.gb_H.gb_qd:hover{background:#93baf9;border-color:transparent;-webkit-box-shadow:0 1px 3px 1px rgba(0,0,0,.15),0 1px 2px rgba(0,0,0,.3);box-shadow:0 1px 3px 1px rgba(0,0,0,.15),0 1px 2px rgba(0,0,0,.3)}#gb .gb_Lc a.gb_qd:focus:not(.gb_H),#gb .gb_Lc a.gb_qd:focus:hover:not(.gb_H),#gb.gb_Lc a.gb_qd:focus:not(.gb_H),#gb.gb_Lc a.gb_qd:focus:hover:not(.gb_H){background:#f4f8ff;outline:1px solid #c9ddfc}#gb a.gb_Ua.gb_H.gb_qd:focus,#gb a.gb_Ua.gb_H.gb_qd:focus:hover{background:#a6c6fa;border-color:transparent;-webkit-box-shadow:none;box-shadow:none}#gb .gb_Lc a.gb_qd:active:not(.gb_H),#gb.gb_Lc a.gb_qd:active{background:#ecf3fe}#gb a.gb_Ua.gb_H.gb_qd:active{background:#a1c3f9;-webkit-box-shadow:0 1px 2px rgba(60,64,67,.3),0 2px 6px 2px rgba(60,64,67,.15);box-shadow:0 1px 2px rgba(60,64,67,.3),0 2px 6px 2px rgba(60,64,67,.15)}.gb_K{display:none}@media screen and (max-width:319px){.gb_ld .gb_J{display:none;visibility:hidden}}.gb_Wa{background-color:rgba(255,255,255,.88);border:1px solid #dadce0;-webkit-box-sizing:border-box;box-sizing:border-box;cursor:pointer;display:inline-block;max-height:48px;overflow:hidden;outline:none;padding:0;vertical-align:middle;width:134px;-webkit-border-radius:8px;border-radius:8px}.gb_Wa.gb_H{background-color:transparent;border:1px solid #5f6368}.gb_3a{display:inherit}.gb_Wa.gb_H .gb_3a{background:#fff;-webkit-border-radius:4px;border-radius:4px;display:inline-block;left:8px;margin-right:5px;position:relative;padding:3px;top:-1px}.gb_Wa:hover{border:1px solid #d2e3fc;background-color:rgba(248,250,255,.88)}.gb_Wa.gb_H:hover{background-color:rgba(241,243,244,.04);border:1px solid #5f6368}.gb_Wa:focus-visible,.gb_Wa:focus{background-color:#fff;outline:1px solid #202124;-webkit-box-shadow:0 1px 2px 0 rgba(60,64,67,.3),0 1px 3px 1px rgba(60,64,67,.15);box-shadow:0 1px 2px 0 rgba(60,64,67,.3),0 1px 3px 1px rgba(60,64,67,.15)}.gb_Wa.gb_H:focus-visible,.gb_Wa.gb_H:focus{background-color:rgba(241,243,244,.12);outline:1px solid #f1f3f4;-webkit-box-shadow:0 1px 3px 1px rgba(0,0,0,.15),0 1px 2px 0 rgba(0,0,0,.3);box-shadow:0 1px 3px 1px rgba(0,0,0,.15),0 1px 2px 0 rgba(0,0,0,.3)}.gb_Wa.gb_H:active,.gb_Wa.gb_Tc.gb_H:focus{background-color:rgba(241,243,244,.1);border:1px solid #5f6368}.gb_4a{display:inline-block;padding-bottom:2px;padding-left:7px;padding-top:2px;text-align:center;vertical-align:middle;line-height:32px;width:78px}.gb_Wa.gb_H .gb_4a{line-height:26px;margin-left:0;padding-bottom:0;padding-left:0;padding-top:0;width:72px}.gb_4a.gb_5a{background-color:#f1f3f4;-webkit-border-radius:4px;border-radius:4px;margin-left:8px;padding-left:0;line-height:30px}.gb_4a.gb_5a .gb_Ic{vertical-align:middle}.gb_Fa:not(.gb_cc) .gb_Wa{margin-left:10px;margin-right:4px}.gb_Sd{max-height:32px;width:78px}.gb_Wa.gb_H .gb_Sd{max-height:26px;width:72px}.gb_P{-webkit-background-size:32px 32px;background-size:32px 32px;border:0;-webkit-border-radius:50%;border-radius:50%;display:block;margin:0px;position:relative;height:32px;width:32px;z-index:0}.gb_eb{background-color:#e8f0fe;border:1px solid rgba(32,33,36,.08);position:relative}.gb_eb.gb_P{height:30px;width:30px}.gb_eb.gb_P:hover,.gb_eb.gb_P:active{-webkit-box-shadow:none;box-shadow:none}.gb_fb{background:#fff;border:none;-webkit-border-radius:50%;border-radius:50%;bottom:2px;-webkit-box-shadow:0px 1px 2px 0px rgba(60,64,67,.30),0px 1px 3px 1px rgba(60,64,67,.15);box-shadow:0px 1px 2px 0px rgba(60,64,67,.30),0px 1px 3px 1px rgba(60,64,67,.15);height:14px;margin:2px;position:absolute;right:0;width:14px}.gb_wc{color:#1f71e7;font:400 22px/32px Google Sans,Roboto,Helvetica,Arial,sans-serif;text-align:center;text-transform:uppercase}@media (-webkit-min-device-pixel-ratio:1.25),(min-resolution:1.25dppx),(min-device-pixel-ratio:1.25){.gb_P::before,.gb_gb::before{display:inline-block;-webkit-transform:scale(0.5);-webkit-transform:scale(0.5);transform:scale(0.5);-webkit-transform-origin:left 0;-webkit-transform-origin:left 0;transform-origin:left 0}.gb_3 .gb_gb::before{-webkit-transform:scale(scale(0.416666667));-webkit-transform:scale(scale(0.416666667));transform:scale(scale(0.416666667))}}.gb_P:hover,.gb_P:focus{-webkit-box-shadow:0 1px 0 rgba(0,0,0,.15);box-shadow:0 1px 0 rgba(0,0,0,.15)}.gb_P:active{-webkit-box-shadow:inset 0 2px 0 rgba(0,0,0,.15);box-shadow:inset 0 2px 0 rgba(0,0,0,.15)}.gb_P:active::after{background:rgba(0,0,0,.1);-webkit-border-radius:50%;border-radius:50%;content:"";display:block;height:100%}.gb_hb{cursor:pointer;line-height:40px;min-width:30px;opacity:.75;overflow:hidden;vertical-align:middle;text-overflow:ellipsis}.gb_B.gb_hb{width:auto}.gb_hb:hover,.gb_hb:focus{opacity:.85}.gb_gd .gb_hb,.gb_gd .gb_Ud{line-height:26px}#gb#gb.gb_gd a.gb_hb,.gb_gd .gb_Ud{font-size:11px;height:auto}.gb_ib{border-top:4px solid #000;border-left:4px dashed transparent;border-right:4px dashed transparent;display:inline-block;margin-left:6px;opacity:.75;vertical-align:middle}.gb_Za:hover .gb_ib{opacity:.85}.gb_Wa>.gb_z{padding:3px 3px 3px 4px}.gb_Vd.gb_nd{color:#fff}.gb_1 .gb_hb,.gb_1 .gb_ib{opacity:1}#gb#gb.gb_1.gb_1 a.gb_hb,#gb#gb .gb_1.gb_1 a.gb_hb{color:#fff}.gb_1.gb_1 .gb_ib{border-top-color:#fff;opacity:1}.gb_ka .gb_P:hover,.gb_1 .gb_P:hover,.gb_ka .gb_P:focus,.gb_1 .gb_P:focus{-webkit-box-shadow:0 1px 0 rgba(0,0,0,.15),0 1px 2px rgba(0,0,0,.2);box-shadow:0 1px 0 rgba(0,0,0,.15),0 1px 2px rgba(0,0,0,.2)}.gb_Wd .gb_z,.gb_Xd .gb_z{position:absolute;right:1px}.gb_z.gb_0,.gb_jb.gb_0,.gb_Za.gb_0{-webkit-flex:0 1 auto;-webkit-box-flex:0;flex:0 1 auto}.gb_Zd.gb_0d .gb_hb{width:30px!important}.gb_1d{height:40px;position:absolute;right:-5px;top:-5px;width:40px}.gb_2d .gb_1d,.gb_3d .gb_1d{right:0;top:0}.gb_z .gb_B{padding:4px}.gb_S{display:none}sentinel{}</style><script nonce="">;this.gbar_={CONFIG:[[[0,"www.gstatic.com","og.qtm.en_US.eebVy_fNKiM.2019.O","com.eg","en","425",0,[4,2,"","","","735207307","0"],null,"yA7SZ__IBceG6-AP5Nqo4AU",null,0,"og.qtm.sDa5bc0wD58.L.W.O","AA2YrTv9PWxAWOkNMB0THY2YxYWamdWWtA","AA2YrTucClwlLUqaQmlTybxGncrc_XS2Pg","",2,1,200,"EGY",null,null,"425","425",1,null,null,114591953,null,0],null,[1,0.1000000014901161,2,1],null,[1,0,0,null,"0","maryamsayed207@gmail.com","","AKeJmwuvLLBHPb-51Tm-fEe3D1ZXjRDxWmG3ZhdtzB-OhGvcfiJp-2n7sgo2XwGs6sCzp1gDntBUsVgqW5VItP1U9TvSV8Fvag",0,0,0,""],[0,0,"",1,0,0,0,0,0,0,null,0,0,null,0,0,null,null,0,0,0,"","","","","","",null,0,0,0,0,0,null,null,null,"rgba(32,33,36,1)","rgba(255,255,255,1)",0,0,0,null,null,null,0],["%1$s (default)","Brand account",1,"%1$s (delegated)",1,null,83,"https://colab.research.google.com/?authuser=$authuser",null,null,null,1,"https://accounts.google.com/ListAccounts?listPages=0\u0026authuser=0\u0026pid=425\u0026gpsia=1\u0026source=ogb\u0026atic=1\u0026mo=1\u0026mn=1\u0026hl=en\u0026ts=250",0,"dashboard",null,null,null,null,"Profile","",1,null,"Signed out","https://accounts.google.com/AccountChooser?source=ogb\u0026continue=$continue\u0026Email=$email\u0026ec=GAhAqQM","https://accounts.google.com/RemoveLocalAccount?source=ogb","Remove","Sign in",0,1,1,0,1,1,0,null,null,null,"Session expired",null,null,null,"Visitor",null,"Default","Delegated","Sign out of all accounts",1,null,null,0,null,null,"myaccount.google.com","https",0,1,0],null,["1","gci_91f30755d6a6b787dcc2a4062e6e9824.js","googleapis.client:gapi.iframes","0","en"],null,null,null,null,["m;/_/scs/abc-static/_/js/k=gapi.gapi.en.uiLLJjqnhCQ.O/d=1/rs=AHpOoo8NP2y291iiPDmfAN0GV3dvCuqlYA/m=__features__","https://apis.google.com","","","1","",null,1,"es_plusone_gc_20250210.0_p0","en",null,0],[0.009999999776482582,"com.eg","425",[null,"","0",null,1,5184000,null,null,"",null,null,null,null,null,0,null,0,null,1,0,0,0,null,null,0,0,null,0,0,0,0,0],null,null,null,0],[1,null,null,40400,425,"EGY","en","735207307.0",8,null,1,0,null,null,null,null,"3700949,3701187,102797341,102797343,102839464,102839466",null,null,null,"yA7SZ__IBceG6-AP5Nqo4AU",0,0,0,null,2,5,"nn",172,0,0,0,0,1,114591953,0,0],[[null,null,null,"https://www.gstatic.com/og/_/js/k=og.qtm.en_US.eebVy_fNKiM.2019.O/rt=j/m=qabr,qgl,q_dnp,qcwid,qbd,qapid,qads,qrcd,q_dg/exm=qaaw,qadd,qaid,qein,qhaw,qhba,qhbr,qhch,qhga,qhid,qhin/d=1/ed=1/rs=AA2YrTv9PWxAWOkNMB0THY2YxYWamdWWtA"],[null,null,null,"https://www.gstatic.com/og/_/ss/k=og.qtm.sDa5bc0wD58.L.W.O/m=qcwid,qba/excm=qaaw,qadd,qaid,qein,qhaw,qhba,qhbr,qhch,qhga,qhid,qhin/d=1/ed=1/ct=zgms/rs=AA2YrTucClwlLUqaQmlTybxGncrc_XS2Pg"]],null,null,null,[[[null,null,[null,null,null,"https://ogs.google.com/u/0/widget/account?yac=1\u0026bac=1\u0026amb=1"],0,414,436,57,4,1,0,0,65,66,8000,"https://accounts.google.com/SignOutOptions?hl=en\u0026continue=https://colab.research.google.com/\u0026ec=GBRAqQM",68,2,null,null,1,113,"Something went wrong.%1$s Refresh to try again or %2$schoose another account%3$s.",3,null,null,75,0,null,null,null,null,null,null,null,"/widget/account",["https","myaccount.google.com",0,32,83,0],0,0,1,["Critical security alert","Important account alert","Storage usage alert",1,1],0,1,null,1,1,1,1,null,null,0,0,0,null,0,0],[null,null,[null,null,null,"https://ogs.google.com/u/0/widget/callout/sid?dc=1"],null,280,420,70,25,0,null,0,null,null,8000,null,71,4,null,null,null,null,null,null,null,null,76,null,null,null,107,108,109,"",null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,0]],null,null,"425","425",1,0,null,"en",0,["https://colab.research.google.com/?authuser=$authuser","https://accounts.google.com/AddSession?hl=en\u0026continue=https://colab.research.google.com/\u0026ec=GAlAqQM","https://accounts.google.com/Logout?hl=en\u0026continue=https://colab.research.google.com/\u0026timeStmp=1741819592\u0026secTok=.AG5fkS_eNFrnYBjrKGLZcfRacF-B4mqMng\u0026ec=GAdAqQM","https://accounts.google.com/ListAccounts?listPages=0\u0026authuser=0\u0026pid=425\u0026gpsia=1\u0026source=ogb\u0026atic=1\u0026mo=1\u0026mn=1\u0026hl=en\u0026ts=250",0,0,"",0,0,null,0,0,"https://accounts.google.com/ServiceLogin?passive=true\u0026continue=https%3A%2F%2Fcolab.research.google.com%2F\u0026ec=GAZAqQM",1,1,0,0,null,0],0,0,0,[null,"",null,null,null,1,null,0,0,"","","","https://ogads-pa.clients6.google.com",0,0,0,"","",0,0,null,86400,null,1,1,null,0,null,0,0,"8559284470"],0,null,null,null,1,0],null,[["mousedown","touchstart","touchmove","wheel","keydown"],300000],[[null,null,null,"https://accounts.google.com/RotateCookiesPage"],3,null,null,null,0,1]]],};this.gbar_=this.gbar_||{};(function(_){var window=this;
try{
_._F_toggles_initialize=function(a){(typeof globalThis!=="undefined"?globalThis:typeof self!=="undefined"?self:this)._F_toggles=a||[]};(0,_._F_toggles_initialize)([]);
/*

 Copyright The Closure Library Authors.
 SPDX-License-Identifier: Apache-2.0
*/
var ca,ka,la,qa,sa,ta,Aa,Ia,Ja,Na,Qa,Ka,Pa,Oa,Ma,La,Ra,hb,lb,ib,mb,xb,yb,zb,Ab;_.aa=function(a,b){if(Error.captureStackTrace)Error.captureStackTrace(this,_.aa);else{const c=Error().stack;c&&(this.stack=c)}a&&(this.message=String(a));b!==void 0&&(this.cause=b)};_.ba=function(a){a.Gj=!0;return a};ca=function(a,b){if(a.length>b.length)return!1;if(a.length<b.length||a===b)return!0;for(let c=0;c<a.length;c++){const d=a[c],e=b[c];if(d>e)return!1;if(d<e)return!0}};
_.ea=function(a){_.t.setTimeout(()=>{throw a;},0)};_.ha=function(){return _.fa().toLowerCase().indexOf("webkit")!=-1};_.fa=function(){var a=_.t.navigator;return a&&(a=a.userAgent)?a:""};ka=function(a){if(!ia||!ja)return!1;for(let b=0;b<ja.brands.length;b++){const {brand:c}=ja.brands[b];if(c&&c.indexOf(a)!=-1)return!0}return!1};_.u=function(a){return _.fa().indexOf(a)!=-1};la=function(){return ia?!!ja&&ja.brands.length>0:!1};_.ma=function(){return la()?!1:_.u("Opera")};
_.oa=function(){return la()?!1:_.u("Trident")||_.u("MSIE")};_.pa=function(){return _.u("Firefox")||_.u("FxiOS")};_.ra=function(){return _.u("Safari")&&!(qa()||(la()?0:_.u("Coast"))||_.ma()||(la()?0:_.u("Edge"))||(la()?ka("Microsoft Edge"):_.u("Edg/"))||(la()?ka("Opera"):_.u("OPR"))||_.pa()||_.u("Silk")||_.u("Android"))};qa=function(){return la()?ka("Chromium"):(_.u("Chrome")||_.u("CriOS"))&&!(la()?0:_.u("Edge"))||_.u("Silk")};sa=function(){return ia?!!ja&&!!ja.platform:!1};
ta=function(){return _.u("iPhone")&&!_.u("iPod")&&!_.u("iPad")};_.ua=function(){return ta()||_.u("iPad")||_.u("iPod")};_.va=function(){return sa()?ja.platform==="macOS":_.u("Macintosh")};_.xa=function(a,b){return _.wa(a,b)>=0};_.ya=function(a){let b="",c=0;const d=a.length-10240;for(;c<d;)b+=String.fromCharCode.apply(null,a.subarray(c,c+=10240));b+=String.fromCharCode.apply(null,c?a.subarray(c):a);return btoa(b)};_.za=function(a){return a!=null&&a instanceof Uint8Array};
Aa=function(a,b){a.__closure__error__context__984382||(a.__closure__error__context__984382={});a.__closure__error__context__984382.severity=b};_.Ba=function(a){a=Error(a);Aa(a,"warning");return a};_.Da=function(a,b){if(a!=null){var c;var d=(c=Ca)!=null?c:Ca={};c=d[a]||0;c>=b||(d[a]=c+1,a=Error(),Aa(a,"incident"),_.ea(a))}};_.Ea=function(a,b=!1){return b&&Symbol.for&&a?Symbol.for(a):a!=null?Symbol(a):Symbol()};_.Fa=function(a,b){a[_.v]&=~b};
_.Ga=function(a){return a!==null&&typeof a==="object"&&!Array.isArray(a)&&a.constructor===Object};_.Ha=function(a){if(a&2)throw Error();};Ia=function(a){return a};Ja=function(a){return a};Na=function(a,b,c,d){return Ka(a,b,c,d,La,Ma)};Qa=function(a,b,c,d){return Ka(a,b,c,d,Oa,Pa)};
Ka=function(a,b,c,d,e,f){if(!c.length&&!d)return 1;var g=0;let h=0,k=0;var l=0;let m=0;for(var n=c.length-1;n>=0;n--){var r=c[n];d&&n===c.length-1&&r===d||(l++,r!=null&&k++)}if(d)for(var q in d)n=+q,isNaN(n)||(m+=Ra(n),h++,n>g&&(g=n));l=e(l,k)+f(h,g,m);q=k;n=h;r=g;let w=m;for(let I=c.length-1;I>=0;I--){var B=c[I];if(B==null||d&&I===c.length-1&&B===d)continue;B=I-b;const N=e(B,q)+f(n,r,w);N<l&&(a=1+B,l=N);n++;q--;w+=Ra(B);r=Math.max(r,B)}b=e(0,0)+f(n,r,w);b<l&&(a=1,l=b);if(d){n=h;r=g;w=m;q=k;for(const I in d)d=
+I,isNaN(d)||d>=1024||(n--,q++,w-=I.length,g=e(d,q)+f(n,r,w),g<l&&(a=1+d,l=g))}return a};Pa=function(a,b,c){return c+a*3+(a>1?a-1:0)};Oa=function(a,b){return(a>1?a-1:0)+(a-b)*4};Ma=function(a,b){return a==0?0:9*Math.max(1<<32-Math.clz32(a+a/2-1),4)<=b?a==0?0:a<4?100+(a-1)*16:a<6?148+(a-4)*16:a<12?244+(a-6)*16:a<22?436+(a-12)*19:a<44?820+(a-22)*17:52+32*a:40+4*b};La=function(a){return 40+4*a};Ra=function(a){return a>=100?a>=1E4?Math.ceil(Math.log10(1+a)):a<1E3?3:4:a<10?1:2};
_.Ta=function(a){if(typeof a!=="boolean")throw Error("s`"+_.Sa(a)+"`"+a);return a};_.Va=function(a){if(!(0,_.Ua)(a))throw _.Ba("enum");return a|0};_.Wa=function(a){if(typeof a!=="number")throw _.Ba("int32");if(!(0,_.Ua)(a))throw _.Ba("int32");return a|0};_.Xa=function(a){if(a!=null&&typeof a!=="string")throw Error();return a};_.Ya=function(a){return a==null||typeof a==="string"?a:void 0};
_.$a=function(a,b,c){if(a!=null&&typeof a==="object"&&a.Ed===_.Za)return a;if(Array.isArray(a)){var d=a[_.v]|0,e=d;e===0&&(e|=c&32);e|=c&2;e!==d&&(a[_.v]=e);return new b(a)}};_.cb=function(a){const b=_.ab(_.bb);return b?a[b]:void 0};
_.fb=function(a,b,c,d,e){const f=d?!!(b&32):void 0;d=[];var g=a.length;let h,k,l,m=!1;if(b&64){if(b&256?(g--,h=a[g],k=g):(k=4294967295,h=void 0),!(e||b&512)){m=!0;var n;l=((n=db)!=null?n:Ja)(h?k- -1:b>>15&1023||536870912,-1,a,h);k=l+-1}}else k=4294967295,b&1||(h=g&&a[g-1],_.Ga(h)?(g--,k=g,l=0):h=void 0);n=void 0;for(let q=0;q<g;q++){let w=a[q];if(w!=null&&(w=c(w,f))!=null)if(q>=k){var r=void 0;((r=n)!=null?r:n={})[q- -1]=w}else d[q]=w}if(h)for(let q in h)if(r=h[q],r!=null&&(r=c(r,f))!=null)if(g=+q,
g<l)d[g+-1]=r;else{let w;((w=n)!=null?w:n={})[q]=r}n&&(m?d.push(n):d[k]=n);e&&(d[_.v]=b&33522241|(n!=null?290:34),_.ab(_.bb)&&(a=_.cb(a))&&"function"==typeof _.eb&&a instanceof _.eb&&(d[_.bb]=a.j()));return d};
hb=function(a){switch(typeof a){case "number":return Number.isFinite(a)?a:""+a;case "bigint":return(0,_.gb)(a)?Number(a):""+a;case "boolean":return a?1:0;case "object":if(Array.isArray(a)){const b=a[_.v]|0;return a.length===0&&b&1?void 0:_.fb(a,b,hb,!1,!1)}if(a.Ed===_.Za)return ib(a);if("function"==typeof _.jb&&a instanceof _.jb)return a.j();if(_.za(a))return _.za(a)&&_.Da(kb,5),_.ya(a);return}return a};lb=function(a,b){if(b){db=b===Ja||b!==Ia&&b!==Na&&b!==Qa?Ja:b;try{return ib(a)}finally{db=void 0}}return ib(a)};
ib=function(a){a=a.ha;return _.fb(a,a[_.v]|0,hb,void 0,!1)};
_.nb=function(a,b,c,d){if(a==null){var e=96;c?(a=[c],e|=512):a=[];b&&(e=e&-33521665|(b&1023)<<15)}else{if(!Array.isArray(a))throw Error("v");e=a[_.v]|0;8192&e||!(64&e)||2&e||mb();if(e&1024)throw Error("x");if(e&64)return d!==3||e&16384||(a[_.v]=e|16384),a;d===1||d===2||(e|=64);if(c&&(e|=512,c!==a[0]))throw Error("y");a:{c=a;var f=c.length;if(f){var g=f-1;const k=c[g];if(_.Ga(k)){e|=256;b=e&512?0:-1;g-=b;if(g>=1024)throw Error("A");for(var h in k)if(f=+h,f<g)c[f+b]=k[h],delete k[h];else break;e=e&
-33521665|(g&1023)<<15;break a}}if(b){h=Math.max(b,f-(e&512?0:-1));if(h>1024)throw Error("B");e=e&-33521665|(h&1023)<<15}}}d===3&&(e|=16384);a[_.v]=e;return a};mb=function(){_.Da(ob,5)};
_.pb=function(a,b){if(typeof a!=="object")return a;if(Array.isArray(a)){const d=a[_.v]|0;if(a.length===0&&d&1)return;if(d&2)return a;var c;if(c=b)c=d===0||!!(d&32)&&!(d&64||!(d&16));return c?(a[_.v]|=34,d&4&&Object.freeze(a),a):_.fb(a,d,_.pb,b!==void 0,!0)}if(a.Ed===_.Za)return b=a.ha,c=b[_.v]|0,c&2?a:_.fb(b,c,_.pb,!0,!0);if("function"==typeof _.jb&&a instanceof _.jb)return a;if(_.za(a))return _.za(a)&&_.Da(kb,5),new Uint8Array(a)};
_.qb=function(a){const b=a.ha;if(!((b[_.v]|0)&2))return a;a=new a.constructor(_.fb(b,b[_.v]|0,_.pb,!0,!0));_.Fa(a.ha,2);return a};_.rb=function(a,b,c,d){const e=b&512?0:-1,f=c+e;var g=a.length-1;if(f>=g&&b&256)return a[g][c]=d,b;if(f<=g)return a[f]=d,b;d!==void 0&&(g=b>>15&1023||536870912,c>=g?d!=null&&(a[g+e]={[c]:d},b|=256,a[_.v]=b):a[f]=d);return b};_.tb=function(a,b,c){a=a.ha;let d=a[_.v]|0;const e=_.sb(a,d,c);b=_.$a(e,b,d);b!==e&&b!=null&&_.rb(a,d,c,b);return b};
_.ub=function(){const a=class{constructor(){throw Error();}};Object.setPrototypeOf(a,a.prototype);return a};_.x=function(a,b){return a!=null?!!a:!!b};_.y=function(a,b){b==void 0&&(b="");return a!=null?a:b};_.vb=function(a,b,c){for(const d in a)b.call(c,a[d],d,a)};_.wb=function(a){for(const b in a)return!1;return!0};xb=Object.defineProperty;
yb=function(a){a=["object"==typeof globalThis&&globalThis,a,"object"==typeof window&&window,"object"==typeof self&&self,"object"==typeof global&&global];for(var b=0;b<a.length;++b){var c=a[b];if(c&&c.Math==Math)return c}throw Error("a");};zb=yb(this);Ab=function(a,b){if(b)a:{var c=zb;a=a.split(".");for(var d=0;d<a.length-1;d++){var e=a[d];if(!(e in c))break a;c=c[e]}a=a[a.length-1];d=c[a];b=b(d);b!=d&&b!=null&&xb(c,a,{configurable:!0,writable:!0,value:b})}};Ab("globalThis",function(a){return a||zb});
Ab("Symbol.dispose",function(a){return a?a:Symbol("b")});Ab("Promise.prototype.finally",function(a){return a?a:function(b){return this.then(function(c){return Promise.resolve(b()).then(function(){return c})},function(c){return Promise.resolve(b()).then(function(){throw c;})})}});
Ab("Array.prototype.flat",function(a){return a?a:function(b){b=b===void 0?1:b;var c=[];Array.prototype.forEach.call(this,function(d){Array.isArray(d)&&b>0?(d=Array.prototype.flat.call(d,b-1),c.push.apply(c,d)):c.push(d)});return c}});var Cb,Gb;_.Bb=_.Bb||{};_.t=this||self;Cb=_.t._F_toggles||[];_.Db=function(a,b){a=a.split(".");b=b||_.t;for(var c=0;c<a.length;c++)if(b=b[a[c]],b==null)return null;return b};_.Sa=function(a){var b=typeof a;return b!="object"?b:a?Array.isArray(a)?"array":b:"null"};_.Eb=function(a){var b=typeof a;return b=="object"&&a!=null||b=="function"};_.Fb="closure_uid_"+(Math.random()*1E9>>>0);Gb=function(a,b,c){return a.call.apply(a.bind,arguments)};_.z=function(a,b,c){_.z=Gb;return _.z.apply(null,arguments)};
_.Hb=function(a,b){var c=Array.prototype.slice.call(arguments,1);return function(){var d=c.slice();d.push.apply(d,arguments);return a.apply(this,d)}};_.A=function(a,b){a=a.split(".");for(var c=_.t,d;a.length&&(d=a.shift());)a.length||b===void 0?c[d]&&c[d]!==Object.prototype[d]?c=c[d]:c=c[d]={}:c[d]=b};_.ab=function(a){return a};
_.C=function(a,b){function c(){}c.prototype=b.prototype;a.X=b.prototype;a.prototype=new c;a.prototype.constructor=a;a.yj=function(d,e,f){for(var g=Array(arguments.length-2),h=2;h<arguments.length;h++)g[h-2]=arguments[h];return b.prototype[e].apply(d,g)}};_.C(_.aa,Error);_.aa.prototype.name="CustomError";_.Ib=_.ba(a=>typeof a==="number");_.Jb=_.ba(a=>typeof a==="string");_.Kb=_.ba(a=>typeof a==="boolean");_.Lb=typeof _.t.BigInt==="function"&&typeof _.t.BigInt(0)==="bigint";var Ob,Mb,Pb,Nb;_.gb=_.ba(a=>_.Lb?a>=Mb&&a<=Nb:a[0]==="-"?ca(a,Ob):ca(a,Pb));Ob=Number.MIN_SAFE_INTEGER.toString();Mb=_.Lb?BigInt(Number.MIN_SAFE_INTEGER):void 0;Pb=Number.MAX_SAFE_INTEGER.toString();Nb=_.Lb?BigInt(Number.MAX_SAFE_INTEGER):void 0;_.Qb=typeof TextDecoder!=="undefined";_.Rb=typeof TextEncoder!=="undefined";var Sb=!!(Cb[0]&2048);var Tb;if(Cb[0]&1024)Tb=Sb;else{var Ub=_.Db("WIZ_global_data.oxN3nb"),Vb=Ub&&Ub[610401301];Tb=Vb!=null?Vb:!1}var ia=Tb;var ja,Wb=_.t.navigator;ja=Wb?Wb.userAgentData||null:null;_.wa=function(a,b){return Array.prototype.indexOf.call(a,b,void 0)};_.Xb=function(a,b,c){Array.prototype.forEach.call(a,b,c)};_.Yb=function(a,b){return Array.prototype.some.call(a,b,void 0)};_.Zb=function(a){_.Zb[" "](a);return a};_.Zb[" "]=function(){};var lc;_.$b=_.ma();_.ac=_.oa();_.bc=_.u("Edge");_.cc=_.u("Gecko")&&!(_.ha()&&!_.u("Edge"))&&!(_.u("Trident")||_.u("MSIE"))&&!_.u("Edge");_.dc=_.ha()&&!_.u("Edge");_.ec=_.va();_.fc=sa()?ja.platform==="Windows":_.u("Windows");_.gc=sa()?ja.platform==="Android":_.u("Android");_.hc=ta();_.ic=_.u("iPad");_.jc=_.u("iPod");_.kc=_.ua();
a:{let a="";const b=function(){const c=_.fa();if(_.cc)return/rv:([^\);]+)(\)|;)/.exec(c);if(_.bc)return/Edge\/([\d\.]+)/.exec(c);if(_.ac)return/\b(?:MSIE|rv)[: ]([^\);]+)(\)|;)/.exec(c);if(_.dc)return/WebKit\/(\S+)/.exec(c);if(_.$b)return/(?:Version)[ \/]?(\S+)/.exec(c)}();b&&(a=b?b[1]:"");if(_.ac){var mc;const c=_.t.document;mc=c?c.documentMode:void 0;if(mc!=null&&mc>parseFloat(a)){lc=String(mc);break a}}lc=a}_.nc=lc;_.oc=_.pa();_.pc=ta()||_.u("iPod");_.qc=_.u("iPad");_.rc=_.u("Android")&&!(qa()||_.pa()||_.ma()||_.u("Silk"));_.sc=qa();_.tc=_.ra()&&!_.ua();var Ca=void 0;var ob,kb;_.bb=_.Ea();_.uc=_.Ea();ob=_.Ea();kb=_.Ea();_.v=_.Ea("jas",!0);var wc;_.Za={};wc=[];wc[_.v]=55;_.vc=Object.freeze(wc);_.xc=Object.freeze({});_.yc=typeof BigInt==="function"?BigInt.asIntN:void 0;_.zc=Number.isSafeInteger;_.Ua=Number.isFinite;_.Ac=Math.trunc;var db;_.Bc=function(a,b){a=a.ha;return _.sb(a,a[_.v]|0,b)};_.sb=function(a,b,c){if(c===-1)return null;const d=c+(b&512?0:-1),e=a.length-1;if(d>=e&&b&256)return a[e][c];if(d<=e)return a[d]};_.Cc=function(a,b,c){const d=a.ha;let e=d[_.v]|0;_.Ha(e);_.rb(d,e,b,c);return a};_.D=function(a,b,c){b=_.tb(a,b,c);if(b==null)return b;a=a.ha;let d=a[_.v]|0;if(!(d&2)){const e=_.qb(b);e!==b&&(b=e,_.rb(a,d,c,b))}return b};_.E=function(a,b,c){c==null&&(c=void 0);return _.Cc(a,b,c)};
_.F=function(a,b){a=_.Bc(a,b);return a==null||typeof a==="boolean"?a:typeof a==="number"?!!a:void 0};_.G=function(a,b){return _.Ya(_.Bc(a,b))};_.H=function(a,b){let c;return(c=_.F(a,b))!=null?c:!1};_.J=function(a,b){let c;return(c=_.G(a,b))!=null?c:""};_.K=function(a,b,c){return _.Cc(a,b,c==null?c:_.Ta(c))};_.L=function(a,b,c){return _.Cc(a,b,c==null?c:_.Wa(c))};_.M=function(a,b,c){return _.Cc(a,b,_.Xa(c))};_.O=function(a,b,c){return _.Cc(a,b,c==null?c:_.Va(c))};_.P=class{constructor(a,b,c){this.ha=_.nb(a,b,c,3)}toJSON(){return lb(this)}ya(a){return JSON.stringify(lb(this,a))}qc(){return!!((this.ha[_.v]|0)&2)}};_.P.prototype.Ed=_.Za;_.P.prototype.toString=function(){return this.ha.toString()};_.Dc=_.ub();_.Ec=_.ub();_.Fc=_.ub();_.Gc=Symbol();var Jc=class extends _.P{constructor(a){super(a)}};_.Kc=class extends _.P{constructor(a){super(a)}D(a){return _.L(this,3,a)}};var Lc=class extends _.P{constructor(a){super(a)}Ic(a){return _.M(this,24,a)}};_.Mc=class extends _.P{constructor(a){super(a)}};_.Q=function(){this.qa=this.qa;this.Y=this.Y};_.Q.prototype.qa=!1;_.Q.prototype.isDisposed=function(){return this.qa};_.Q.prototype.dispose=function(){this.qa||(this.qa=!0,this.P())};_.Q.prototype[Symbol.dispose]=function(){this.dispose()};_.Q.prototype.P=function(){if(this.Y)for(;this.Y.length;)this.Y.shift()()};var Nc=class extends _.Q{constructor(){var a=window;super();this.o=a;this.i=[];this.j={}}resolve(a){let b=this.o;a=a.split(".");const c=a.length;for(let d=0;d<c;++d)if(b[a[d]])b=b[a[d]];else return null;return b instanceof Function?b:null}ob(){const a=this.i.length,b=this.i,c=[];for(let d=0;d<a;++d){const e=b[d].i(),f=this.resolve(e);if(f&&f!=this.j[e])try{b[d].ob(f)}catch(g){}else c.push(b[d])}this.i=c.concat(b.slice(a))}};var Pc=class extends _.Q{constructor(){var a=_.Oc;super();this.o=a;this.A=this.i=null;this.v=0;this.B={};this.j=!1;a=window.navigator.userAgent;a.indexOf("MSIE")>=0&&a.indexOf("Trident")>=0&&(a=/\b(?:MSIE|rv)[: ]([^\);]+)(\)|;)/.exec(a))&&a[1]&&parseFloat(a[1])<9&&(this.j=!0)}C(a,b){this.i=b;this.A=a;b.preventDefault?b.preventDefault():b.returnValue=!1}};_.Qc=class extends _.P{constructor(a){super(a)}};var Rc=class extends _.P{constructor(a){super(a)}};var Tc;_.Sc=function(a,b,c=98,d=new _.Kc){if(a.i){const e=new Jc;_.M(e,1,b.message);_.M(e,2,b.stack);_.L(e,3,b.lineNumber);_.O(e,5,1);_.E(d,40,e);a.i.log(c,d)}};Tc=class{constructor(){this.i=null}log(a,b,c=new _.Kc){_.Sc(this,a,98,c)}};var Uc,Vc;Uc=function(a){if(a.o.length>0){var b=a.i!==void 0,c=a.j!==void 0;if(b||c){b=b?a.v:a.A;c=a.o;a.o=[];try{_.Xb(c,b,a)}catch(d){console.error(d)}}}};_.Wc=class{constructor(a){this.i=a;this.j=void 0;this.o=[]}then(a,b,c){this.o.push(new Vc(a,b,c));Uc(this)}resolve(a){if(this.i!==void 0||this.j!==void 0)throw Error("F");this.i=a;Uc(this)}reject(a){if(this.i!==void 0||this.j!==void 0)throw Error("F");this.j=a;Uc(this)}v(a){a.j&&a.j.call(a.i,this.i)}A(a){a.o&&a.o.call(a.i,this.j)}};
Vc=class{constructor(a,b,c){this.j=a;this.o=b;this.i=c}};_.Xc=a=>{var b="lc";if(a.lc&&a.hasOwnProperty(b))return a.lc;b=new a;return a.lc=b};_.R=class{constructor(){this.v=new _.Wc;this.i=new _.Wc;this.D=new _.Wc;this.B=new _.Wc;this.C=new _.Wc;this.A=new _.Wc;this.o=new _.Wc;this.j=new _.Wc;this.F=new _.Wc}Y(){return this.v}M(){return this.i}N(){return this.D}L(){return this.B}qa(){return this.C}K(){return this.A}J(){return this.o}G(){return this.j}static i(){return _.Xc(_.R)}};var ad;_.Zc=function(){return _.D(_.Yc,Lc,1)};_.$c=function(){return _.D(_.Yc,_.Mc,5)};ad=class extends _.P{constructor(a){super(a)}};var bd;window.gbar_&&window.gbar_.CONFIG?bd=window.gbar_.CONFIG[0]||{}:bd=[];_.Yc=new ad(bd);_.D(_.Yc,Rc,3)||new Rc;_.Zc()||new Lc;_.Oc=new Tc;_.A("gbar_._DumpException",function(a){_.Oc?_.Oc.log(a):console.error(a)});_.cd=new Pc;var ed;_.fd=function(a,b){var c=_.dd.i();if(a in c.i){if(c.i[a]!=b)throw new ed;}else{c.i[a]=b;const h=c.j[a];if(h)for(let k=0,l=h.length;k<l;k++){b=h[k];var d=c.i;delete b.i[a];if(_.wb(b.i)){for(var e=b.j.length,f=Array(e),g=0;g<e;g++)f[g]=d[b.j[g]];b.o.apply(b.v,f)}}delete c.j[a]}};_.dd=class{constructor(){this.i={};this.j={}}static i(){return _.Xc(_.dd)}};_.gd=class extends _.aa{constructor(){super()}};ed=class extends _.gd{};_.A("gbar.A",_.Wc);_.Wc.prototype.aa=_.Wc.prototype.then;_.A("gbar.B",_.R);_.R.prototype.ba=_.R.prototype.M;_.R.prototype.bb=_.R.prototype.N;_.R.prototype.bd=_.R.prototype.qa;_.R.prototype.bf=_.R.prototype.Y;_.R.prototype.bg=_.R.prototype.L;_.R.prototype.bh=_.R.prototype.K;_.R.prototype.bj=_.R.prototype.J;_.R.prototype.bk=_.R.prototype.G;_.A("gbar.a",_.R.i());window.gbar&&window.gbar.ap&&window.gbar.ap(window.gbar.a);var hd=new Nc;_.fd("api",hd);var id=_.$c()||new _.Mc;window.__PVT=_.y(_.G(id,8));
_.fd("eq",_.cd);
}catch(e){_._DumpException(e)}
try{
_.jd=class extends _.P{constructor(a){super(a)}};
}catch(e){_._DumpException(e)}
try{
var kd=class extends _.P{constructor(a){super(a)}};var ld=class extends _.Q{constructor(){super();this.j=[];this.i=[]}o(a,b){this.j.push({features:a,options:b!=null?b:null})}init(a,b,c){window.gapi={};const d=window.___jsl={};d.h=_.y(_.G(a,1));_.F(a,12)!=null&&(d.dpo=_.x(_.H(a,12)));d.ms=_.y(_.G(a,2));d.m=_.y(_.G(a,3));d.l=[];_.J(b,1)&&(a=_.G(b,3))&&this.i.push(a);_.J(c,1)&&(c=_.G(c,2))&&this.i.push(c);_.A("gapi.load",(0,_.z)(this.o,this));return this}};var md=_.D(_.Yc,_.Qc,14);if(md){var nd=_.D(_.Yc,_.jd,9)||new _.jd,od=new kd,pd=new ld;pd.init(md,nd,od);_.fd("gs",pd)};
}catch(e){_._DumpException(e)}
})(this.gbar_);
// Google Inc.
</script><script nonce="">try {const preferences = JSON.parse(window.localStorage.getItem("datalab_prefs_maryamsayed207@gmail.com")); document.querySelector('html') .setAttribute('theme', preferences['siteTheme'] || 'default');} catch (e) {}</script><script nonce="">window.performance.mark('head_start');</script><link rel="stylesheet" href="./Untitled21.ipynb - Colab_files/bundle.css"><script nonce="">var colabVersionTag = 'colab_20250311-060133_RC00_735676493'; var colabScsVersion = 'e9e71e9458cc628437d9ad4cbd7a1be2'; var hl = 'en'; var colabExperiments = JSON.parse('\x7b\x22add_df_vars_in_ai_conversation_context\x22: false, \x22add_prompt_cell\x22: false, \x22agent_scroll_delay_ms\x22: 200, \x22ai_banner\x22: false, \x22ai_unsubscribed_warning\x22: false, \x22ai_user_input_char_limit\x22: 2000, \x22aida_complete_code_model_id\x22: \x22\x22, \x22aida_converse_max_facts\x22: 20, \x22aida_do_conversation_model_id\x22: \x22\x22, \x22aida_generate_code_model_id\x22: \x22\x22, \x22allow_dsa_page_interaction\x22: true, \x22allow_readonly_cells\x22: true, \x22allowed_public_url_domains\x22: \x5b\x22huggingface.co\x22, \x22dagshub.com\x22, \x22storage.googleapis.com\x22\x5d, \x22auto_open_chat_on_empty_notebook\x22: false, \x22backend_url_allowlist\x22: \x5b\x22localhost\x22, \x22127.0.0.1\x22, \x22\x5b::1\x5d\x22, \x22kkb-production.jupyter-proxy.kaggle.net\x22\x5d, \x22backend_version\x22: \x22next\x22, \x22backtracking_strategy\x22: \x22non-literals\x22, \x22cell_markdown_toolbar_tooltips\x22: true, \x22cell_output_actions_tooltip\x22: true, \x22cell_tags\x22: false, \x22cell_toolbar_ai_menu\x22: true, \x22cell_toolbar_tooltips\x22: true, \x22cell_ui_refresh\x22: false, \x22chat_explain_error_temp\x22: \x221.0\x22, \x22chat_model_id_override\x22: \x22\x22, \x22chat_reduce_refusals\x22: true, \x22classified_generate\x22: false, \x22classroom_iframe_parent_origin\x22: \x22\x22, \x22client_text_compose\x22: true, \x22client_trim_completion_text\x22: 400, \x22cloud_origin\x22: \x22\x22, \x22code_report_millis\x22: 600000, \x22commands_in_toolbar\x22: true, \x22comment_poll_long\x22: 900000, \x22comment_poll_short\x22: 60000, \x22compose_skip_suffix_check\x22: false, \x22composer\x22: false, \x22converse_server_side_history\x22: false, \x22converse_temp\x22: \x22\x22, \x22corp_third_party_widgets\x22: false, \x22crawler\x22: false, \x22create_gemini_api_key\x22: false, \x22critique_comments\x22: false, \x22dbu\x22: \x22\x22, \x22debug_external\x22: \x22external\x22, \x22debug_prod\x22: \x22prod\x22, \x22dep_cells_commands\x22: true, \x22dep_cells_enabled\x22: false, \x22dep_graph\x22: false, \x22deprecate_prompt\x22: false, \x22development\x22: false, \x22document_change_poll_interval\x22: 30000, \x22drive_anon_api_key\x22: \x22AIzaSyB10s2vWUTwP0pj20wZoxmpZIt3rRodYeg\x22, \x22drive_api_key\x22: \x22AIzaSyCN_sSPJMpYrAzC5AtTrltNC8oRmLtoqBk\x22, \x22drive_background_save_project_number\x22: \x22948411933973\x22, \x22drive_realtime_project_number\x22: \x22\x22, \x22drop_chat_links\x22: true, \x22dsa\x22: true, \x22dsa_sample_datasets_toast\x22: true, \x22embedding_app\x22: \x22\x22, \x22enable_adhoc_backends\x22: false, \x22enable_agent_connect_to_new_vm\x22: true, \x22enable_completions_backend_switching\x22: false, \x22enable_dasher_subscription_ui\x22: true, \x22enable_more_reprs\x22: true, \x22enable_mpp_orc_model_overrides\x22: true, \x22enable_rt_on_create\x22: false, \x22execution_announcements\x22: true, \x22execution_status_propagation\x22: true, \x22explain_cell\x22: true, \x22explain_error\x22: true, \x22explain_error_model_id_override\x22: \x22\x22, \x22explain_error_trim_traceback\x22: true, \x22explicit_ai_backend\x22: \x22\x22, \x22external_trusted_github_org_repos_quick_add\x22: \x22GoogleChrome\/CrUX,google\/generative-ai-docs,google-health\/cxr-foundation,google-health\/derm-foundation,google-health\/path-foundation\x22, \x22file_browser_poll_interval_millis\x22: 10000, \x22file_upload_rate_limit\x22: 5, \x22filter_repetitive_suggestions\x22: false, \x22first_party_auth\x22: true, \x22fix_imports\x22: false, \x22generate_code\x22: true, \x22generate_df\x22: true, \x22generate_prompt_reduce_blank_responses\x22: false, \x22generate_prompt_reduce_name_errors\x22: false, \x22generate_temp\x22: \x22\x22, \x22get_started\x22: false, \x22gis_auth\x22: true, \x22github_client_id\x22: \x225036cf6d81e65aaa6340\x22, \x22gpu_utilization_check_interval_ms\x22: 600000, \x22granular_browser_permissions\x22: true, \x22hats_surveys\x22: true, \x22hrc\x22: false, \x22i18n_runtime_labels\x22: true, \x22import_data\x22: false, \x22import_gemini_api_key\x22: true, \x22include_df_vars_in_ai_conversation_context\x22: false, \x22inline_completion_ai_campaign_max_views\x22: 3, \x22inline_completion_ai_campaign_throttle_ms\x22: 600000, \x22interactive_sheet_next_steps\x22: true, \x22is_prober\x22: false, \x22jsraw\x22: \x22compiled\x22, \x22key_promoter\x22: false, \x22kr\x22: false, \x22latest_notebook_context_for_converse\x22: true, \x22link_id_assignments\x22: true, \x22link_imports_to_installs\x22: true, \x22local_cloud_apis\x22: false, \x22local_service_worker\x22: false, \x22lsp_diagnostics_reporting\x22: false, \x22lsp_inlay_hint\x22: false, \x22makersuite_api_key\x22: \x22AIzaSyAmDcruecW4rCL1KdwcbIVHL4LkXxahIgw\x22, \x22makersuite_service_url\x22: \x22https:\/\/alkalimakersuite-pa.clients6.google.com\x22, \x22markdown_spellchecker\x22: false, \x22min_dep_cells_runtime_kernel_cl\x22: 694609395, \x22ml_enabled\x22: true, \x22mlpp_multiline\x22: false, \x22mobile\x22: false, \x22mpp_orc_temperature_override\x22: \x221.0\x22, \x22next_steps\x22: true, \x22nl2code_missing_imports\x22: false, \x22no_fun\x22: false, \x22notebook_context_length\x22: 40000, \x22outage_notification\x22: \x22\x22, \x22outage_notification_link\x22: \x22\x22, \x22outputframe_version\x22: \x22\x22, \x22override_suf_params_for_test\x22: false, \x22parallel_prompting\x22: true, \x22pds_minting\x22: false, \x22prereq_cells_next_steps\x22: true, \x22prevent_ai_long_response_generate\x22: false, \x22prevent_ai_long_response_generate_with_df\x22: false, \x22prevent_ai_long_response_suggest_fix\x22: false, \x22prompt_for_dsa_trusted_tester_consent\x22: false, \x22recaptcha_polling_frequency_ms\x22: 300000, \x22recaptcha_v2_site_key\x22: \x226LfQttQUAAAAADuPanA_VZMaZgBAOnHZNuuqUewp\x22, \x22recaptcha_v3_site_key\x22: \x226LfQPtEUAAAAAHBpAdFng54jyuB1V5w5dofknpip\x22, \x22reconnect_max_delay_seconds\x22: 300, \x22remove_ai_explain_cell_fencing\x22: true, \x22remove_ai_explain_error_fencing\x22: true, \x22remove_ai_generate_fencing\x22: true, \x22require_ai_consent\x22: true, \x22resource_poll_interval_ms\x22: 10000, \x22rp_kws\x22: true, \x22rp_kxhr_skip_fallback\x22: false, \x22rp_serve_kernel_port\x22: false, \x22rp_socketio_fallback\x22: true, \x22rp_token_refresh_headroom_millis\x22: 300000, \x22rt_opt_in\x22: \x22OFF\x22, \x22run_mode\x22: false, \x22runtime_env_overrides\x22: \x22\\n          \x5b\\n            \x5b\\\x22ENABLE_DIRECTORYPREFETCHER\\\x22, \\\x221\\\x22\x5d\\n          \x5d\\n        \x22, \x22runtime_type_for_test\x22: \x22\x22, \x22server_execution_queue\x22: true, \x22server_side_generate_prompt_formatting_cloud\x22: false, \x22session_resume_coalesce\x22: true, \x22show_empty_notebook_actions\x22: true, \x22show_gemini_button_text_label\x22: false, \x22show_payments_interstitial\x22: false, \x22show_rel_notes_on_open\x22: true, \x22show_signup_survey\x22: true, \x22show_subscription_renewal_time\x22: false, \x22show_switch_to_prod_link\x22: false, \x22single_page_consent_form\x22: true, \x22smartpaste\x22: false, \x22smartpaste_serving_config\x22: \x22pl_700m_smart_paste_3.0.32_60\x22, \x22sql_cell\x22: false, \x22sql_cell_buttons\x22: false, \x22storage_partition_trial\x22: true, \x22storage_partition_trial_token\x22: \x22Agk\/t4Bt05W7j6CHeqXH9+6ccDayrBsQPqCLDPSElphe\/7cUobayuvN0A3huajTbJenIjp6qibLteh6e0IEWrgIAAAB4eyJvcmlnaW4iOiJodHRwczovL2NvbGFiLnJlc2VhcmNoLmdvb2dsZS5jb206NDQzIiwiZmVhdHVyZSI6IkRpc2FibGVUaGlyZFBhcnR5U3RvcmFnZVBhcnRpdGlvbmluZzIiLCJleHBpcnkiOjE3NDIzNDIzOTl9\x22, \x22task_service_max_poll_count\x22: 45, \x22task_service_poll_interval_ms\x22: 2000, \x22task_service_wait_before_polling_ms\x22: 5000, \x22term4all\x22: false, \x22terminate_session_on_connect_to_new_vm\x22: false, \x22text_compose_report_changes_millis\x22: 10000, \x22text_span_comments\x22: false, \x22toolbar_above_left_pane\x22: true, \x22tpu_node_redirect\x22: true, \x22tpu_resource_stats\x22: false, \x22tpu_v5e1\x22: true, \x22transform_code\x22: false, \x22transform_code_context_file_per_cell\x22: false, \x22turn_off_agent_mode_when_safe\x22: true, \x22unmanaged_vm_min_label_block\x22: \x22\x22, \x22unmanaged_vm_min_label_warn\x22: \x22\x22, \x22unmanaged_vm_min_release_tag_block\x22: \x22\x22, \x22unmanaged_vm_min_release_tag_warn\x22: \x22\x22, \x22unsupported_magics_check\x22: true, \x22updated_inline_cell_diff\x22: false, \x22use_corplogin\x22: true, \x22use_tpu_eligibility_lists\x22: false, \x22user_visible_accelerator_models\x22: \x5b\x22T4\x22, \x22A100\x22, \x22L4\x22, \x22V28\x22, \x22V5E1\x22\x5d, \x22user_visible_gpu_types\x22: \x5b\x22T4\x22, \x22A100\x22, \x22L4\x22\x5d, \x22v_100_redirect\x22: true, \x22verbose_warnings\x22: false, \x22vertex_ai_api_environment_override\x22: \x22\x22, \x22want_completions_ai_consent_campaign\x22: true, \x22workstations\x22: false, \x22ids\x22: \x5b20730182, 20730315, 20730363, 20730374, 20730230, 20730186, 20730369, 20730265, 20730150, 20730324, 20730177, 20730297\x5d, \x22flag_ids\x22: \x7b\x22add_df_vars_in_ai_conversation_context\x22: 45678289, \x22add_prompt_cell\x22: 45644995, \x22agent_scroll_delay_ms\x22: 45680776, \x22ai_banner\x22: 45670540, \x22ai_unsubscribed_warning\x22: 45504730, \x22ai_user_input_char_limit\x22: 45661098, \x22aida_complete_code_model_id\x22: 45427660, \x22aida_converse_max_facts\x22: 45680037, \x22aida_do_conversation_model_id\x22: 45427664, \x22aida_generate_code_model_id\x22: 45427663, \x22allow_dsa_page_interaction\x22: 45675785, \x22allow_readonly_cells\x22: 45671718, \x22allowed_public_url_domains\x22: 45425558, \x22auto_open_chat_on_empty_notebook\x22: 45669599, \x22backend_url_allowlist\x22: 45660303, \x22backend_version\x22: 45425541, \x22backtracking_strategy\x22: 45644832, \x22cell_markdown_toolbar_tooltips\x22: 45654223, \x22cell_output_actions_tooltip\x22: 45650940, \x22cell_tags\x22: 45425779, \x22cell_toolbar_ai_menu\x22: 45647581, \x22cell_toolbar_tooltips\x22: 45649981, \x22cell_ui_refresh\x22: 45673630, \x22chat_explain_error_temp\x22: 45655973, \x22chat_model_id_override\x22: 45631876, \x22chat_reduce_refusals\x22: 45656767, \x22classified_generate\x22: 45425499, \x22classroom_iframe_parent_origin\x22: 45425537, \x22client_text_compose\x22: 45425512, \x22client_trim_completion_text\x22: 45425628, \x22cloud_origin\x22: 45425538, \x22code_report_millis\x22: 45658073, \x22commands_in_toolbar\x22: 45425502, \x22comment_poll_long\x22: 45425588, \x22comment_poll_short\x22: 45425587, \x22compose_skip_suffix_check\x22: 45615470, \x22composer\x22: 45683351, \x22converse_server_side_history\x22: 45634472, \x22converse_temp\x22: 45425509, \x22corp_third_party_widgets\x22: 45678906, \x22crawler\x22: 45425491, \x22create_gemini_api_key\x22: 45654552, \x22critique_comments\x22: 45612076, \x22dbu\x22: 45425545, \x22debug_external\x22: 45425470, \x22debug_prod\x22: 45425471, \x22dep_cells_commands\x22: 45622249, \x22dep_cells_enabled\x22: 45653551, \x22dep_graph\x22: 45629071, \x22deprecate_prompt\x22: 45679897, \x22development\x22: 45425544, \x22document_change_poll_interval\x22: 45425589, \x22drive_anon_api_key\x22: 45425478, \x22drive_api_key\x22: 45425473, \x22drive_background_save_project_number\x22: 45425479, \x22drive_realtime_project_number\x22: 45425629, \x22drop_chat_links\x22: 45646864, \x22dsa\x22: 45656258, \x22dsa_sample_datasets_toast\x22: 45682045, \x22enable_adhoc_backends\x22: 45425506, \x22enable_agent_connect_to_new_vm\x22: 45670252, \x22enable_completions_backend_switching\x22: 45662651, \x22enable_dasher_subscription_ui\x22: 45639531, \x22enable_more_reprs\x22: 45613354, \x22enable_mpp_orc_model_overrides\x22: 45649913, \x22enable_rt_on_create\x22: 45667583, \x22execution_announcements\x22: 45651325, \x22execution_status_propagation\x22: 45644828, \x22explain_cell\x22: 45425505, \x22explain_error\x22: 45425487, \x22explain_error_model_id_override\x22: 45631875, \x22explain_error_trim_traceback\x22: 45618831, \x22explicit_ai_backend\x22: 45638548, \x22external_trusted_github_org_repos_quick_add\x22: 45425555, \x22file_browser_poll_interval_millis\x22: 45643722, \x22file_upload_rate_limit\x22: 45637799, \x22filter_repetitive_suggestions\x22: 45615781, \x22first_party_auth\x22: 45425560, \x22fix_imports\x22: 45624140, \x22generate_code\x22: 45425492, \x22generate_df\x22: 45425503, \x22generate_prompt_reduce_blank_responses\x22: 45643396, \x22generate_prompt_reduce_name_errors\x22: 45634392, \x22generate_temp\x22: 45425508, \x22get_started\x22: 45430267, \x22gis_auth\x22: 45425625, \x22github_client_id\x22: 45425556, \x22gpu_utilization_check_interval_ms\x22: 45425561, \x22granular_browser_permissions\x22: 45630936, \x22hats_surveys\x22: 45425559, \x22i18n_runtime_labels\x22: 45662916, \x22import_data\x22: 45430411, \x22import_gemini_api_key\x22: 45654551, \x22include_df_vars_in_ai_conversation_context\x22: 45676033, \x22inline_completion_ai_campaign_max_views\x22: 45676328, \x22inline_completion_ai_campaign_throttle_ms\x22: 45671534, \x22interactive_sheet_next_steps\x22: 45634324, \x22is_prober\x22: 45429104, \x22jsraw\x22: 45425557, \x22key_promoter\x22: 45425570, \x22latest_notebook_context_for_converse\x22: 45668776, \x22link_id_assignments\x22: 45644831, \x22link_imports_to_installs\x22: 45644830, \x22local_cloud_apis\x22: 45425630, \x22local_service_worker\x22: 45425550, \x22lsp_diagnostics_reporting\x22: 45425604, \x22lsp_inlay_hint\x22: 45614695, \x22makersuite_api_key\x22: 45655361, \x22makersuite_service_url\x22: 45655362, \x22markdown_spellchecker\x22: 45671479, \x22min_dep_cells_runtime_kernel_cl\x22: 45654240, \x22ml_enabled\x22: 45425493, \x22mlpp_multiline\x22: 45425623, \x22mobile\x22: 45425562, \x22mpp_orc_temperature_override\x22: 45649914, \x22next_steps\x22: 45428239, \x22nl2code_missing_imports\x22: 45615676, \x22no_fun\x22: 45425540, \x22notebook_context_length\x22: 45633457, \x22outage_notification\x22: 45425584, \x22outage_notification_link\x22: 45425585, \x22outputframe_version\x22: 45425591, \x22override_suf_params_for_test\x22: 45425592, \x22parallel_prompting\x22: 45666384, \x22pds_minting\x22: 45648255, \x22prereq_cells_next_steps\x22: 45640400, \x22prevent_ai_long_response_generate\x22: 45680972, \x22prevent_ai_long_response_generate_with_df\x22: 45681123, \x22prevent_ai_long_response_suggest_fix\x22: 45681124, \x22prompt_for_dsa_trusted_tester_consent\x22: 45670923, \x22recaptcha_polling_frequency_ms\x22: 45425582, \x22recaptcha_v2_site_key\x22: 45425581, \x22recaptcha_v3_site_key\x22: 45425580, \x22reconnect_max_delay_seconds\x22: 45425539, \x22remove_ai_explain_cell_fencing\x22: 45677303, \x22remove_ai_explain_error_fencing\x22: 45677302, \x22remove_ai_generate_fencing\x22: 45673079, \x22require_ai_consent\x22: 45425489, \x22resource_poll_interval_ms\x22: 45425590, \x22rp_kws\x22: 45650184, \x22rp_kxhr_skip_fallback\x22: 45656329, \x22rp_serve_kernel_port\x22: 45572083, \x22rp_socketio_fallback\x22: 45658495, \x22rp_token_refresh_headroom_millis\x22: 45517773, \x22rt_opt_in\x22: 45667546, \x22run_mode\x22: 45642857, \x22runtime_env_overrides\x22: 45425583, \x22runtime_type_for_test\x22: 45425586, \x22server_execution_queue\x22: 45425600, \x22server_side_generate_prompt_formatting_cloud\x22: 45655196, \x22session_resume_coalesce\x22: 45425603, \x22show_empty_notebook_actions\x22: 45677304, \x22show_gemini_button_text_label\x22: 45681647, \x22show_payments_interstitial\x22: 45425543, \x22show_rel_notes_on_open\x22: 45644210, \x22show_signup_survey\x22: 45425620, \x22show_subscription_renewal_time\x22: 45425569, \x22show_switch_to_prod_link\x22: 45425483, \x22single_page_consent_form\x22: 45656775, \x22smartpaste\x22: 45627425, \x22smartpaste_serving_config\x22: 45630585, \x22sql_cell\x22: 45425497, \x22sql_cell_buttons\x22: 45425498, \x22task_service_max_poll_count\x22: 45669592, \x22task_service_poll_interval_ms\x22: 45669591, \x22task_service_wait_before_polling_ms\x22: 45669590, \x22term4all\x22: 45425542, \x22terminate_session_on_connect_to_new_vm\x22: 45683597, \x22text_compose_report_changes_millis\x22: 45425568, \x22text_span_comments\x22: 45545873, \x22toolbar_above_left_pane\x22: 45683504, \x22tpu_node_redirect\x22: 45634372, \x22tpu_resource_stats\x22: 45655215, \x22tpu_v5e1\x22: 45652002, \x22transform_code\x22: 45667102, \x22transform_code_context_file_per_cell\x22: 45671260, \x22turn_off_agent_mode_when_safe\x22: 45679577, \x22unmanaged_vm_min_label_block\x22: 45425546, \x22unmanaged_vm_min_label_warn\x22: 45425547, \x22unmanaged_vm_min_release_tag_block\x22: 45425548, \x22unmanaged_vm_min_release_tag_warn\x22: 45425549, \x22unsupported_magics_check\x22: 45644829, \x22updated_inline_cell_diff\x22: 45667103, \x22use_corplogin\x22: 45425606, \x22use_tpu_eligibility_lists\x22: 45682573, \x22user_visible_accelerator_models\x22: 45682571, \x22user_visible_gpu_types\x22: 45620529, \x22v_100_redirect\x22: 45644963, \x22verbose_warnings\x22: 45425551, \x22vertex_ai_api_environment_override\x22: 45612077, \x22want_completions_ai_consent_campaign\x22: 45671138, \x22workstations\x22: 45425626\x7d\x7d'); var colabUserEmail = 'maryamsayed207@gmail.com'; var colabRenderDataToken = 'AFWLbD1dxdURj8JTvhwLRQ8fTtPtPhBysutCDVRlGlayRxoeOShbjkcJZQCoja-XBKgS5MsHoe4Cn5oj9nMiOKmhEZRA3TEGJfsN'; var colabConfig = '\x5b\x5b\x22maryamsayed207@gmail.com\x22,\x5b1,\x22AHXL0D1mchu8EHxL5X3QpcXgPvuhZFzaiknuY8SM+jnMqZfob2ROcXUfp2aMQnfL9X97cESWcOA0sr2KrbaONZNVT5TmCZUqmptkQGD6RhLcaH+cfXMnPXUSG8Uk0ABF0WhMbP2Psiv8HkMyUqpqcukjUxu9HAobwr43PgEeKsiwrw2f1jGJBvsZYUbiTvSv7eVkeL29b5fiskdIwI9HbcktXyayPC4QXEv5cOAbirXcn7P9m5MIumph41Ky3mLjkQ17HHjjpK0T8HvxWdmq7fEH65ccrL92wfR6ktx5AfMfhH2aACs7XD9BZTDNWyFq\/tDHT1f1Uh2YhvekNlKdtlvQaW7q4LI1RdnmnnNEJt3YOOeX0w0KK3PjQgyhfRBkmIdfsRsajgmJyAs3GtVhF0u095a1N+Kx\/EjCiEdJOQiwZkscIx5JLiYp8G92Ra41v7tS9pcuNYAjsb6mpm8t9Q1UecQezIoCNJJ2adgNPFteedNBUoE9Y+IqzVYm435FCyYWn7IRWJ2vhl8ZzZSqPB3LEXoPQd5lMTIXnbbDILDGfBDv5qG6ZemwPYqyggbi3floZyedIhZvL2MnU3ZmzQLNiaDaI28FwjQbq\/b7JT0aAK3rzfZsyy7e2vPUJAoBXp+rSZVEXWHh2YMlGnmUPVMQ1\/N8UluRadvz4qmnPfuKVDFxPoJHz4hlNo7ncdUGoUEiG\/qWuBkWmIqd3vzqo6MXijaS3vynU5ILPSw+OUx4IMHDFjujEXHrqb+H5mjEfmnC1tO0CDaUdhFTo+ZAshm6eInbkWTBPGlVBJr1Gky1lW0Jiko4H\/kRuDuReUcU\/Uj\/3tzcIoAJRgQA50ydz4M+sxxcT\/aSwWWj6DyjSHYgQCOd64kmAT67S5s9MFMcqJ4SvDP2OQ4Wa0zxD9NBX23Fj6tYnII1Gy7CzcXUrAHc79OFQrdKRnQnIqGXny9jvRWPEwiNGTz1Oze0l+bHP9JL4ygifzo2EKFue1TctbrA4+SIxhYf5TIKj7X9oks7Sau6AxOGM0w\/tVDbwW6MlkoQ2iokcrGSPDHhGS+ec60lVOHSo1VhnnZ3Y7RP\/XrH4kAOgb95mRMV1\/NK\/dHZugdFXyd17HrdOY4aUmyGaDn2S86spBXmY7zzU5uXGBcPjpw\/WCsLYqvHNjn6RfeZi7HZEX+EhDiqQOo5MiSVs8AN1NKFWfW8mVtAVLO0FbPG6FZtfTs\/3UjmRdiYyQ+zljm5JPwg6cg+lLcV8q\/oehxjIzLSu9PgSau2BI07RUWVXRtrS6onJXOf4kpRrM3jlLGMwxOz4Xn+9THVtRi5fLol46BWCJura4\/2o5t0E7VPvH+dNm6U3g8g6NYpyMbReFT74l9Oaa0uj3EOgvG4Gi2EbG4rlC4+5kkJ7iJmy4hG6CJTZOED3mgca2Xt+eVzMmUSnTpFaLam1llCr+9Msk5KDQRWDQG4EayzDG5mg3E7dQeiRKViO2xMQ\/6cKFauubkdbwLBq\/D9oqCwlURCLxpQEheyozRhN4qjFz1epfeF+873cf24i01v12tKPvK\/yJoystnUjUUdgR+ItY3WQOvwZo5gwG+l1eUE9Hqtzs+7Ps2L\/yg54QlQ1\/Yj6IDZzNMFh6N2LWkLQwT9JkGyUGBhRPT9V44rBnt+TsdG7Vk0GfjvxEl6gPJ06fWh4LSB0tNVEKqADBrttHBZVVByZr8fF94wewavowUEoVWo7vRwl3ddM8B+1oNkcMw1OejnRkA+\/vj5cZJeIY96MWzwdwjQfo02vwvXxnJFhCnZ2phvg64C7IctmDBQh8xhK+A5z9C2W+wijk5OpniKDQ4NIEz1MnDqIcC2tujRnuUO9TgOzV0MiJnQaxKj9b5kQK1NB3hcn1iy2zPfykyd6jT810u3dT5xfG1CMNA\x3d\x22,\x22AJ9oCCxNwXDsUM25NVtLDFT3gyGbAZ5yU+OeOGkn8hSJZkMbx3Ie8sumTfa6avRr6nL53M\/78PRrpi7N\/atxC4uHzOnAxHydrchw+wKWgFNvXaTBWOn\/ctksSgJAx2U7226i0kb7VMB6\x22,\x22https:\/\/payments.google.com\/payments\x22,0,0,null,null,null,\x22US$ 9.99\x22,\x22US$ 49.99\x22,\x22US$ 9.99\x22,\x22US$ 49.99\x22\x5d,\x5b1,5\x5d,\x22EG\x22,0\x5d\x5d';</script><link id="favicon-link" rel="shortcut icon" href="https://ssl.gstatic.com/colaboratory-static/common/e9e71e9458cc628437d9ad4cbd7a1be2/img%2Ffavicon.ico"><meta name="google-site-verification" content="wRgpUU3mIRZPD1GORBPNonaotM72092B_DsqQFWNa4s"><meta name="google-site-verification" content="f5qdvL6RAXlBgHezvCLpPtvx2wU5ZgIzzPULroprlnA"><meta name="google-site-verification" content="sNOroO9gXrazN-oMODOm0Bs0_vw1R5QwZ-BfrSHn8Io"><meta name="google-site-verification" content="K1UdZBHJXQYnJGXIK1KuutmVy6dn3vG2sEyV9D1C6dM"><meta name="google-site-verification" content="wdGthzzfu0IjM3qpFqTuQL9poAQZAvAaFKyuzetLpIM"><meta name="google-site-verification" content="qZJ77guHGO0TObHUBRYVdXQlIhXBBuz8dahJVmIlzCo"><meta name="google-site-verification" content="7ahoeOOKT2ZR781GZ5xK4L9t7yO1ZOHc-gaoUALEYgw"><meta name="google-site-verification" content="PHgaSKwdxZELS21aixtLhfpvaHtKen9pnVJ25EI35Zs"><meta name="google-site-verification" content="qylwTsZSLomIg1JrChne7cPcXmtC2Xh_5ZxlJWLlAH0"><meta name="google-site-verification" content="BQfukMqFy1nu2Q2gjGbNTDA8MJ_Y4L2brCYA1h6ewkY"><meta name="google-site-verification" content="Ozey1ptWUQW13_lCEhpPMOcmRBLqdyB3WEL-TJUjskU"><meta name="google-site-verification" content="rF5iXzWe9KZXJes1dQNhOUkS4_z_e97IrsVoCx2trek"><meta name="google-site-verification" content="z-WR3zzv8XZ5FFfBLLDbyTiN35UXm01nWUS2Uej5pwg"><meta name="google-site-verification" content="vsXaeD7OD0m3iK8Z54fG8TYGC5eT17KeL_xMHtdiyWI"><meta name="google-site-verification" content="cpB5oulaGwqSxsg4E-9q2MVbK87iE9NAUUVxdveucPw"><meta name="google-site-verification" content="8P-D5fVWgUIhw8X2BxnKJbf5itK0zxX0QhoBjbJFTe8"><meta name="google-site-verification" content="88fgsZDoVRBuRnDPMIEjcHCxsEXzODOqEsJoqtvQsDc"><meta name="google-site-verification" content="sMarhZgb4va_L_7UTdMR43gDZ2gVqc_5GHN4REpQPGY"><meta name="google-site-verification" content="26aKGBCw3XblB5Ou01UhxY5WDtMqHjoTm6P-lvF6AqE"><meta name="google-site-verification" content="DGionF7db9g0dOgeBXwOAN2tmCzWBdo5yOdc_-5UcuE"><meta name="google-site-verification" content="Q9LlidR0toR7UtSyVO23xNeaqJmRp8I6r4ghBQTtntU"><meta name="google-site-verification" content="rQawcZaTEK_UrDG30cz_7nVKOVvBass61QEes0Tm04g"><meta name="google-site-verification" content="8L3ghjzKIj241AYAmEygniTe604tsXFkIrb1v-DBtGo"><meta name="google-site-verification" content="Gz6pcDgVFH_aS-aPTYW21rSHcWl0LAgKCWJtdXPVTNo"><meta name="google-site-verification" content="KiunYPvrY5x8umvAWcjhwPrB677xCar2LeT_8yaVrDg"><meta name="google-site-verification" content="LypEVvHhYiLSzDs9PabhmOmsfMfEjVGq2rLXJbtqdzY"><meta name="google-site-verification" content="b6bOMRzMVX2bJABYDGBPtpGcB_AUZ-o2SOTggQXErkg"><meta name="google-site-verification" content="v2MQvJk6wTiBarKTbe1mdivqYCVtw-5m6w0HDzV5X_4"><meta name="google-site-verification" content="-N1hdkiHJQ6kwJALkHVh2ZzV2fFNER0schZl2AU6zvc"><meta name="google-site-verification" content="dsf7CRwnDkQv6Ot4gXTXx8_nVf8A9cb5o30hZ7cGAIo"><meta property="og:type" content="article"><meta property="og:image" content="https://colab.research.google.com/img/colab_favicon_256px.png"><meta property="og:title" content="Google Colab"><meta http-equiv="origin-trial" content="Agk/t4Bt05W7j6CHeqXH9+6ccDayrBsQPqCLDPSElphe/7cUobayuvN0A3huajTbJenIjp6qibLteh6e0IEWrgIAAAB4eyJvcmlnaW4iOiJodHRwczovL2NvbGFiLnJlc2VhcmNoLmdvb2dsZS5jb206NDQzIiwiZmVhdHVyZSI6IkRpc2FibGVUaGlyZFBhcnR5U3RvcmFnZVBhcnRpdGlvbmluZzIiLCJleHBpcnkiOjE3NDIzNDIzOTl9"><script nonce="">window.performance.mark('head_end'); window.performance.measure('head', 'head_start', 'head_end');</script><script async="" src="./Untitled21.ipynb - Colab_files/lazy.min.js.download" nonce=""></script><style id="inert-style">
[inert] {
  pointer-events: none;
  cursor: default;
}

[inert], [inert] * {
  user-select: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
}
</style><script async="" type="text/javascript" charset="UTF-8" src="./Untitled21.ipynb - Colab_files/rs=AA2YrTv9PWxAWOkNMB0THY2YxYWamdWWtA" nonce=""></script><link type="text/css" href="./Untitled21.ipynb - Colab_files/rs=AA2YrTucClwlLUqaQmlTybxGncrc_XS2Pg" rel="stylesheet"><style type="text/css">@import url('https://fonts.googleapis.com/css2?family=Work+Sans:ital,wght@0,100..900;1,100..900&display=swap');</style><style type="text/css">.MathJax_Hover_Frame {border-radius: .25em; -webkit-border-radius: .25em; -moz-border-radius: .25em; -khtml-border-radius: .25em; box-shadow: 0px 0px 15px #83A; -webkit-box-shadow: 0px 0px 15px #83A; -moz-box-shadow: 0px 0px 15px #83A; -khtml-box-shadow: 0px 0px 15px #83A; border: 1px solid #A6D ! important; display: inline-block; position: absolute}
.MathJax_Menu_Button .MathJax_Hover_Arrow {position: absolute; cursor: pointer; display: inline-block; border: 2px solid #AAA; border-radius: 4px; -webkit-border-radius: 4px; -moz-border-radius: 4px; -khtml-border-radius: 4px; font-family: 'Courier New',Courier; font-size: 9px; color: #F0F0F0}
.MathJax_Menu_Button .MathJax_Hover_Arrow span {display: block; background-color: #AAA; border: 1px solid; border-radius: 3px; line-height: 0; padding: 4px}
.MathJax_Hover_Arrow:hover {color: white!important; border: 2px solid #CCC!important}
.MathJax_Hover_Arrow:hover span {background-color: #CCC!important}
</style><style type="text/css">#MathJax_About {position: fixed; left: 50%; width: auto; text-align: center; border: 3px outset; padding: 1em 2em; background-color: #DDDDDD; color: black; cursor: default; font-family: message-box; font-size: 120%; font-style: normal; text-indent: 0; text-transform: none; line-height: normal; letter-spacing: normal; word-spacing: normal; word-wrap: normal; white-space: nowrap; float: none; z-index: 201; border-radius: 15px; -webkit-border-radius: 15px; -moz-border-radius: 15px; -khtml-border-radius: 15px; box-shadow: 0px 10px 20px #808080; -webkit-box-shadow: 0px 10px 20px #808080; -moz-box-shadow: 0px 10px 20px #808080; -khtml-box-shadow: 0px 10px 20px #808080; filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=2, OffY=2, Color='gray', Positive='true')}
#MathJax_About.MathJax_MousePost {outline: none}
.MathJax_Menu {position: absolute; background-color: white; color: black; width: auto; padding: 2px; border: 1px solid #CCCCCC; margin: 0; cursor: default; font: menu; text-align: left; text-indent: 0; text-transform: none; line-height: normal; letter-spacing: normal; word-spacing: normal; word-wrap: normal; white-space: nowrap; float: none; z-index: 201; box-shadow: 0px 10px 20px #808080; -webkit-box-shadow: 0px 10px 20px #808080; -moz-box-shadow: 0px 10px 20px #808080; -khtml-box-shadow: 0px 10px 20px #808080; filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=2, OffY=2, Color='gray', Positive='true')}
.MathJax_MenuItem {padding: 2px 2em; background: transparent}
.MathJax_MenuArrow {position: absolute; right: .5em; padding-top: .25em; color: #666666; font-size: .75em}
.MathJax_MenuActive .MathJax_MenuArrow {color: white}
.MathJax_MenuArrow.RTL {left: .5em; right: auto}
.MathJax_MenuCheck {position: absolute; left: .7em}
.MathJax_MenuCheck.RTL {right: .7em; left: auto}
.MathJax_MenuRadioCheck {position: absolute; left: 1em}
.MathJax_MenuRadioCheck.RTL {right: 1em; left: auto}
.MathJax_MenuLabel {padding: 2px 2em 4px 1.33em; font-style: italic}
.MathJax_MenuRule {border-top: 1px solid #CCCCCC; margin: 4px 1px 0px}
.MathJax_MenuDisabled {color: GrayText}
.MathJax_MenuActive {background-color: Highlight; color: HighlightText}
.MathJax_MenuDisabled:focus, .MathJax_MenuLabel:focus {background-color: #E8E8E8}
.MathJax_ContextMenu:focus {outline: none}
.MathJax_ContextMenu .MathJax_MenuItem:focus {outline: none}
#MathJax_AboutClose {top: .2em; right: .2em}
.MathJax_Menu .MathJax_MenuClose {top: -10px; left: -10px}
.MathJax_MenuClose {position: absolute; cursor: pointer; display: inline-block; border: 2px solid #AAA; border-radius: 18px; -webkit-border-radius: 18px; -moz-border-radius: 18px; -khtml-border-radius: 18px; font-family: 'Courier New',Courier; font-size: 24px; color: #F0F0F0}
.MathJax_MenuClose span {display: block; background-color: #AAA; border: 1.5px solid; border-radius: 18px; -webkit-border-radius: 18px; -moz-border-radius: 18px; -khtml-border-radius: 18px; line-height: 0; padding: 8px 0 6px}
.MathJax_MenuClose:hover {color: white!important; border: 2px solid #CCC!important}
.MathJax_MenuClose:hover span {background-color: #CCC!important}
.MathJax_MenuClose:hover:focus {outline: none}
</style><style type="text/css">.MJX_Assistive_MathML {position: absolute!important; top: 0; left: 0; clip: rect(1px, 1px, 1px, 1px); padding: 1px 0 0 0!important; border: 0!important; height: 1px!important; width: 1px!important; overflow: hidden!important; display: block!important; -webkit-touch-callout: none; -webkit-user-select: none; -khtml-user-select: none; -moz-user-select: none; -ms-user-select: none; user-select: none}
.MJX_Assistive_MathML.MJX_Assistive_MathML_Block {width: 100%!important}
</style><style type="text/css">#MathJax_Zoom {position: absolute; background-color: #F0F0F0; overflow: auto; display: block; z-index: 301; padding: .5em; border: 1px solid black; margin: 0; font-weight: normal; font-style: normal; text-align: left; text-indent: 0; text-transform: none; line-height: normal; letter-spacing: normal; word-spacing: normal; word-wrap: normal; white-space: nowrap; float: none; -webkit-box-sizing: content-box; -moz-box-sizing: content-box; box-sizing: content-box; box-shadow: 5px 5px 15px #AAAAAA; -webkit-box-shadow: 5px 5px 15px #AAAAAA; -moz-box-shadow: 5px 5px 15px #AAAAAA; -khtml-box-shadow: 5px 5px 15px #AAAAAA; filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=2, OffY=2, Color='gray', Positive='true')}
#MathJax_ZoomOverlay {position: absolute; left: 0; top: 0; z-index: 300; display: inline-block; width: 100%; height: 100%; border: 0; padding: 0; margin: 0; background-color: white; opacity: 0; filter: alpha(opacity=0)}
#MathJax_ZoomFrame {position: relative; display: inline-block; height: 0; width: 0}
#MathJax_ZoomEventTrap {position: absolute; left: 0; top: 0; z-index: 302; display: inline-block; border: 0; padding: 0; margin: 0; background-color: white; opacity: 0; filter: alpha(opacity=0)}
</style><style type="text/css">.MathJax_Preview {color: #888}
#MathJax_Message {position: fixed; left: 1em; bottom: 1.5em; background-color: #E6E6E6; border: 1px solid #959595; margin: 0px; padding: 2px 8px; z-index: 102; color: black; font-size: 80%; width: auto; white-space: nowrap}
#MathJax_MSIE_Frame {position: absolute; top: 0; left: 0; width: 0px; z-index: 101; border: 0px; margin: 0px; padding: 0px}
.MathJax_Error {color: #CC0000; font-style: italic}
</style><style type="text/css">.MJXp-script {font-size: .8em}
.MJXp-right {-webkit-transform-origin: right; -moz-transform-origin: right; -ms-transform-origin: right; -o-transform-origin: right; transform-origin: right}
.MJXp-bold {font-weight: bold}
.MJXp-italic {font-style: italic}
.MJXp-scr {font-family: MathJax_Script,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-frak {font-family: MathJax_Fraktur,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-sf {font-family: MathJax_SansSerif,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-cal {font-family: MathJax_Caligraphic,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-mono {font-family: MathJax_Typewriter,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-largeop {font-size: 150%}
.MJXp-largeop.MJXp-int {vertical-align: -.2em}
.MJXp-math {display: inline-block; line-height: 1.2; text-indent: 0; font-family: 'Times New Roman',Times,STIXGeneral,serif; white-space: nowrap; border-collapse: collapse}
.MJXp-display {display: block; text-align: center; margin: 1em 0}
.MJXp-math span {display: inline-block}
.MJXp-box {display: block!important; text-align: center}
.MJXp-box:after {content: " "}
.MJXp-rule {display: block!important; margin-top: .1em}
.MJXp-char {display: block!important}
.MJXp-mo {margin: 0 .15em}
.MJXp-mfrac {margin: 0 .125em; vertical-align: .25em}
.MJXp-denom {display: inline-table!important; width: 100%}
.MJXp-denom > * {display: table-row!important}
.MJXp-surd {vertical-align: top}
.MJXp-surd > * {display: block!important}
.MJXp-script-box > *  {display: table!important; height: 50%}
.MJXp-script-box > * > * {display: table-cell!important; vertical-align: top}
.MJXp-script-box > *:last-child > * {vertical-align: bottom}
.MJXp-script-box > * > * > * {display: block!important}
.MJXp-mphantom {visibility: hidden}
.MJXp-munderover, .MJXp-munder {display: inline-table!important}
.MJXp-over {display: inline-block!important; text-align: center}
.MJXp-over > * {display: block!important}
.MJXp-munderover > *, .MJXp-munder > * {display: table-row!important}
.MJXp-mtable {vertical-align: .25em; margin: 0 .125em}
.MJXp-mtable > * {display: inline-table!important; vertical-align: middle}
.MJXp-mtr {display: table-row!important}
.MJXp-mtd {display: table-cell!important; text-align: center; padding: .5em 0 0 .5em}
.MJXp-mtr > .MJXp-mtd:first-child {padding-left: 0}
.MJXp-mtr:first-child > .MJXp-mtd {padding-top: 0}
.MJXp-mlabeledtr {display: table-row!important}
.MJXp-mlabeledtr > .MJXp-mtd:first-child {padding-left: 0}
.MJXp-mlabeledtr:first-child > .MJXp-mtd {padding-top: 0}
.MJXp-merror {background-color: #FFFF88; color: #CC0000; border: 1px solid #CC0000; padding: 1px 3px; font-style: normal; font-size: 90%}
.MJXp-scale0 {-webkit-transform: scaleX(.0); -moz-transform: scaleX(.0); -ms-transform: scaleX(.0); -o-transform: scaleX(.0); transform: scaleX(.0)}
.MJXp-scale1 {-webkit-transform: scaleX(.1); -moz-transform: scaleX(.1); -ms-transform: scaleX(.1); -o-transform: scaleX(.1); transform: scaleX(.1)}
.MJXp-scale2 {-webkit-transform: scaleX(.2); -moz-transform: scaleX(.2); -ms-transform: scaleX(.2); -o-transform: scaleX(.2); transform: scaleX(.2)}
.MJXp-scale3 {-webkit-transform: scaleX(.3); -moz-transform: scaleX(.3); -ms-transform: scaleX(.3); -o-transform: scaleX(.3); transform: scaleX(.3)}
.MJXp-scale4 {-webkit-transform: scaleX(.4); -moz-transform: scaleX(.4); -ms-transform: scaleX(.4); -o-transform: scaleX(.4); transform: scaleX(.4)}
.MJXp-scale5 {-webkit-transform: scaleX(.5); -moz-transform: scaleX(.5); -ms-transform: scaleX(.5); -o-transform: scaleX(.5); transform: scaleX(.5)}
.MJXp-scale6 {-webkit-transform: scaleX(.6); -moz-transform: scaleX(.6); -ms-transform: scaleX(.6); -o-transform: scaleX(.6); transform: scaleX(.6)}
.MJXp-scale7 {-webkit-transform: scaleX(.7); -moz-transform: scaleX(.7); -ms-transform: scaleX(.7); -o-transform: scaleX(.7); transform: scaleX(.7)}
.MJXp-scale8 {-webkit-transform: scaleX(.8); -moz-transform: scaleX(.8); -ms-transform: scaleX(.8); -o-transform: scaleX(.8); transform: scaleX(.8)}
.MJXp-scale9 {-webkit-transform: scaleX(.9); -moz-transform: scaleX(.9); -ms-transform: scaleX(.9); -o-transform: scaleX(.9); transform: scaleX(.9)}
.MathJax_PHTML .noError {vertical-align: ; font-size: 90%; text-align: left; color: black; padding: 1px 3px; border: 1px solid}
</style><style type="text/css">.MathJax_Display {text-align: center; margin: 0; position: relative; display: block!important; text-indent: 0; max-width: none; max-height: none; min-width: 0; min-height: 0; width: 100%}
.MathJax .merror {background-color: #FFFF88; color: #CC0000; border: 1px solid #CC0000; padding: 1px 3px; font-style: normal; font-size: 90%}
.MathJax .MJX-monospace {font-family: monospace}
.MathJax .MJX-sans-serif {font-family: sans-serif}
#MathJax_Tooltip {background-color: InfoBackground; color: InfoText; border: 1px solid black; box-shadow: 2px 2px 5px #AAAAAA; -webkit-box-shadow: 2px 2px 5px #AAAAAA; -moz-box-shadow: 2px 2px 5px #AAAAAA; -khtml-box-shadow: 2px 2px 5px #AAAAAA; filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=2, OffY=2, Color='gray', Positive='true'); padding: 3px 4px; z-index: 401; position: absolute; left: 0; top: 0; width: auto; height: auto; display: none}
.MathJax {display: inline; font-style: normal; font-weight: normal; line-height: normal; font-size: 100%; font-size-adjust: none; text-indent: 0; text-align: left; text-transform: none; letter-spacing: normal; word-spacing: normal; word-wrap: normal; white-space: nowrap; float: none; direction: ltr; max-width: none; max-height: none; min-width: 0; min-height: 0; border: 0; padding: 0; margin: 0}
.MathJax:focus, body :focus .MathJax {display: inline-table}
.MathJax.MathJax_FullWidth {text-align: center; display: table-cell!important; width: 10000em!important}
.MathJax img, .MathJax nobr, .MathJax a {border: 0; padding: 0; margin: 0; max-width: none; max-height: none; min-width: 0; min-height: 0; vertical-align: 0; line-height: normal; text-decoration: none}
img.MathJax_strut {border: 0!important; padding: 0!important; margin: 0!important; vertical-align: 0!important}
.MathJax span {display: inline; position: static; border: 0; padding: 0; margin: 0; vertical-align: 0; line-height: normal; text-decoration: none; box-sizing: content-box}
.MathJax nobr {white-space: nowrap!important}
.MathJax img {display: inline!important; float: none!important}
.MathJax * {transition: none; -webkit-transition: none; -moz-transition: none; -ms-transition: none; -o-transition: none}
.MathJax_Processing {visibility: hidden; position: fixed; width: 0; height: 0; overflow: hidden}
.MathJax_Processed {display: none!important}
.MathJax_test {font-style: normal; font-weight: normal; font-size: 100%; font-size-adjust: none; text-indent: 0; text-transform: none; letter-spacing: normal; word-spacing: normal; overflow: hidden; height: 1px}
.MathJax_test.mjx-test-display {display: table!important}
.MathJax_test.mjx-test-inline {display: inline!important; margin-right: -1px}
.MathJax_test.mjx-test-default {display: block!important; clear: both}
.MathJax_ex_box {display: inline-block!important; position: absolute; overflow: hidden; min-height: 0; max-height: none; padding: 0; border: 0; margin: 0; width: 1px; height: 60ex}
.MathJax_em_box {display: inline-block!important; position: absolute; overflow: hidden; min-height: 0; max-height: none; padding: 0; border: 0; margin: 0; width: 1px; height: 60em}
.mjx-test-inline .MathJax_left_box {display: inline-block; width: 0; float: left}
.mjx-test-inline .MathJax_right_box {display: inline-block; width: 0; float: right}
.mjx-test-display .MathJax_right_box {display: table-cell!important; width: 10000em!important; min-width: 0; max-width: none; padding: 0; border: 0; margin: 0}
.MathJax .MathJax_HitBox {cursor: text; background: white; opacity: 0; filter: alpha(opacity=0)}
.MathJax .MathJax_HitBox * {filter: none; opacity: 1; background: transparent}
#MathJax_Tooltip * {filter: none; opacity: 1; background: transparent}
@font-face {font-family: MathJax_Main; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Main-Regular.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Main-Regular.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Main-bold; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Main-Bold.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Main-Bold.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Main-italic; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Main-Italic.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Main-Italic.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Math-italic; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Math-Italic.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Math-Italic.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Caligraphic; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Caligraphic-Regular.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Caligraphic-Regular.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Size1; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Size1-Regular.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Size1-Regular.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Size2; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Size2-Regular.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Size2-Regular.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Size3; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Size3-Regular.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Size3-Regular.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Size4; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Size4-Regular.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Size4-Regular.otf?V=2.7.5') format('opentype')}
.MathJax .noError {vertical-align: ; font-size: 90%; text-align: left; color: black; padding: 1px 3px; border: 1px solid}
</style><script async="async" type="text/javascript" src="./Untitled21.ipynb - Colab_files/editor.main.js.download"></script><link rel="stylesheet" type="text/css" data-name="vs/editor/editor.main" href="./Untitled21.ipynb - Colab_files/editor.main.css"><script async="async" type="text/javascript" src="./Untitled21.ipynb - Colab_files/editor.main.nls.js.download"></script><script src="./Untitled21.ipynb - Colab_files/api.js.download" nonce=""></script><script src="./Untitled21.ipynb - Colab_files/api(1).js.download" nonce=""></script><style type="text/css" media="screen" class="monaco-colors">.codicon-add:before { content: '\ea60'; }
.codicon-plus:before { content: '\ea60'; }
.codicon-gist-new:before { content: '\ea60'; }
.codicon-repo-create:before { content: '\ea60'; }
.codicon-lightbulb:before { content: '\ea61'; }
.codicon-light-bulb:before { content: '\ea61'; }
.codicon-repo:before { content: '\ea62'; }
.codicon-repo-delete:before { content: '\ea62'; }
.codicon-gist-fork:before { content: '\ea63'; }
.codicon-repo-forked:before { content: '\ea63'; }
.codicon-git-pull-request:before { content: '\ea64'; }
.codicon-git-pull-request-abandoned:before { content: '\ea64'; }
.codicon-record-keys:before { content: '\ea65'; }
.codicon-keyboard:before { content: '\ea65'; }
.codicon-tag:before { content: '\ea66'; }
.codicon-tag-add:before { content: '\ea66'; }
.codicon-tag-remove:before { content: '\ea66'; }
.codicon-person:before { content: '\ea67'; }
.codicon-person-follow:before { content: '\ea67'; }
.codicon-person-outline:before { content: '\ea67'; }
.codicon-person-filled:before { content: '\ea67'; }
.codicon-git-branch:before { content: '\ea68'; }
.codicon-git-branch-create:before { content: '\ea68'; }
.codicon-git-branch-delete:before { content: '\ea68'; }
.codicon-source-control:before { content: '\ea68'; }
.codicon-mirror:before { content: '\ea69'; }
.codicon-mirror-public:before { content: '\ea69'; }
.codicon-star:before { content: '\ea6a'; }
.codicon-star-add:before { content: '\ea6a'; }
.codicon-star-delete:before { content: '\ea6a'; }
.codicon-star-empty:before { content: '\ea6a'; }
.codicon-comment:before { content: '\ea6b'; }
.codicon-comment-add:before { content: '\ea6b'; }
.codicon-alert:before { content: '\ea6c'; }
.codicon-warning:before { content: '\ea6c'; }
.codicon-search:before { content: '\ea6d'; }
.codicon-search-save:before { content: '\ea6d'; }
.codicon-log-out:before { content: '\ea6e'; }
.codicon-sign-out:before { content: '\ea6e'; }
.codicon-log-in:before { content: '\ea6f'; }
.codicon-sign-in:before { content: '\ea6f'; }
.codicon-eye:before { content: '\ea70'; }
.codicon-eye-unwatch:before { content: '\ea70'; }
.codicon-eye-watch:before { content: '\ea70'; }
.codicon-circle-filled:before { content: '\ea71'; }
.codicon-primitive-dot:before { content: '\ea71'; }
.codicon-close-dirty:before { content: '\ea71'; }
.codicon-debug-breakpoint:before { content: '\ea71'; }
.codicon-debug-breakpoint-disabled:before { content: '\ea71'; }
.codicon-debug-hint:before { content: '\ea71'; }
.codicon-primitive-square:before { content: '\ea72'; }
.codicon-edit:before { content: '\ea73'; }
.codicon-pencil:before { content: '\ea73'; }
.codicon-info:before { content: '\ea74'; }
.codicon-issue-opened:before { content: '\ea74'; }
.codicon-gist-private:before { content: '\ea75'; }
.codicon-git-fork-private:before { content: '\ea75'; }
.codicon-lock:before { content: '\ea75'; }
.codicon-mirror-private:before { content: '\ea75'; }
.codicon-close:before { content: '\ea76'; }
.codicon-remove-close:before { content: '\ea76'; }
.codicon-x:before { content: '\ea76'; }
.codicon-repo-sync:before { content: '\ea77'; }
.codicon-sync:before { content: '\ea77'; }
.codicon-clone:before { content: '\ea78'; }
.codicon-desktop-download:before { content: '\ea78'; }
.codicon-beaker:before { content: '\ea79'; }
.codicon-microscope:before { content: '\ea79'; }
.codicon-vm:before { content: '\ea7a'; }
.codicon-device-desktop:before { content: '\ea7a'; }
.codicon-file:before { content: '\ea7b'; }
.codicon-file-text:before { content: '\ea7b'; }
.codicon-more:before { content: '\ea7c'; }
.codicon-ellipsis:before { content: '\ea7c'; }
.codicon-kebab-horizontal:before { content: '\ea7c'; }
.codicon-mail-reply:before { content: '\ea7d'; }
.codicon-reply:before { content: '\ea7d'; }
.codicon-organization:before { content: '\ea7e'; }
.codicon-organization-filled:before { content: '\ea7e'; }
.codicon-organization-outline:before { content: '\ea7e'; }
.codicon-new-file:before { content: '\ea7f'; }
.codicon-file-add:before { content: '\ea7f'; }
.codicon-new-folder:before { content: '\ea80'; }
.codicon-file-directory-create:before { content: '\ea80'; }
.codicon-trash:before { content: '\ea81'; }
.codicon-trashcan:before { content: '\ea81'; }
.codicon-history:before { content: '\ea82'; }
.codicon-clock:before { content: '\ea82'; }
.codicon-folder:before { content: '\ea83'; }
.codicon-file-directory:before { content: '\ea83'; }
.codicon-symbol-folder:before { content: '\ea83'; }
.codicon-logo-github:before { content: '\ea84'; }
.codicon-mark-github:before { content: '\ea84'; }
.codicon-github:before { content: '\ea84'; }
.codicon-terminal:before { content: '\ea85'; }
.codicon-console:before { content: '\ea85'; }
.codicon-repl:before { content: '\ea85'; }
.codicon-zap:before { content: '\ea86'; }
.codicon-symbol-event:before { content: '\ea86'; }
.codicon-error:before { content: '\ea87'; }
.codicon-stop:before { content: '\ea87'; }
.codicon-variable:before { content: '\ea88'; }
.codicon-symbol-variable:before { content: '\ea88'; }
.codicon-array:before { content: '\ea8a'; }
.codicon-symbol-array:before { content: '\ea8a'; }
.codicon-symbol-module:before { content: '\ea8b'; }
.codicon-symbol-package:before { content: '\ea8b'; }
.codicon-symbol-namespace:before { content: '\ea8b'; }
.codicon-symbol-object:before { content: '\ea8b'; }
.codicon-symbol-method:before { content: '\ea8c'; }
.codicon-symbol-function:before { content: '\ea8c'; }
.codicon-symbol-constructor:before { content: '\ea8c'; }
.codicon-symbol-boolean:before { content: '\ea8f'; }
.codicon-symbol-null:before { content: '\ea8f'; }
.codicon-symbol-numeric:before { content: '\ea90'; }
.codicon-symbol-number:before { content: '\ea90'; }
.codicon-symbol-structure:before { content: '\ea91'; }
.codicon-symbol-struct:before { content: '\ea91'; }
.codicon-symbol-parameter:before { content: '\ea92'; }
.codicon-symbol-type-parameter:before { content: '\ea92'; }
.codicon-symbol-key:before { content: '\ea93'; }
.codicon-symbol-text:before { content: '\ea93'; }
.codicon-symbol-reference:before { content: '\ea94'; }
.codicon-go-to-file:before { content: '\ea94'; }
.codicon-symbol-enum:before { content: '\ea95'; }
.codicon-symbol-value:before { content: '\ea95'; }
.codicon-symbol-ruler:before { content: '\ea96'; }
.codicon-symbol-unit:before { content: '\ea96'; }
.codicon-activate-breakpoints:before { content: '\ea97'; }
.codicon-archive:before { content: '\ea98'; }
.codicon-arrow-both:before { content: '\ea99'; }
.codicon-arrow-down:before { content: '\ea9a'; }
.codicon-arrow-left:before { content: '\ea9b'; }
.codicon-arrow-right:before { content: '\ea9c'; }
.codicon-arrow-small-down:before { content: '\ea9d'; }
.codicon-arrow-small-left:before { content: '\ea9e'; }
.codicon-arrow-small-right:before { content: '\ea9f'; }
.codicon-arrow-small-up:before { content: '\eaa0'; }
.codicon-arrow-up:before { content: '\eaa1'; }
.codicon-bell:before { content: '\eaa2'; }
.codicon-bold:before { content: '\eaa3'; }
.codicon-book:before { content: '\eaa4'; }
.codicon-bookmark:before { content: '\eaa5'; }
.codicon-debug-breakpoint-conditional-unverified:before { content: '\eaa6'; }
.codicon-debug-breakpoint-conditional:before { content: '\eaa7'; }
.codicon-debug-breakpoint-conditional-disabled:before { content: '\eaa7'; }
.codicon-debug-breakpoint-data-unverified:before { content: '\eaa8'; }
.codicon-debug-breakpoint-data:before { content: '\eaa9'; }
.codicon-debug-breakpoint-data-disabled:before { content: '\eaa9'; }
.codicon-debug-breakpoint-log-unverified:before { content: '\eaaa'; }
.codicon-debug-breakpoint-log:before { content: '\eaab'; }
.codicon-debug-breakpoint-log-disabled:before { content: '\eaab'; }
.codicon-briefcase:before { content: '\eaac'; }
.codicon-broadcast:before { content: '\eaad'; }
.codicon-browser:before { content: '\eaae'; }
.codicon-bug:before { content: '\eaaf'; }
.codicon-calendar:before { content: '\eab0'; }
.codicon-case-sensitive:before { content: '\eab1'; }
.codicon-check:before { content: '\eab2'; }
.codicon-checklist:before { content: '\eab3'; }
.codicon-chevron-down:before { content: '\eab4'; }
.codicon-drop-down-button:before { content: '\eab4'; }
.codicon-chevron-left:before { content: '\eab5'; }
.codicon-chevron-right:before { content: '\eab6'; }
.codicon-chevron-up:before { content: '\eab7'; }
.codicon-chrome-close:before { content: '\eab8'; }
.codicon-chrome-maximize:before { content: '\eab9'; }
.codicon-chrome-minimize:before { content: '\eaba'; }
.codicon-chrome-restore:before { content: '\eabb'; }
.codicon-circle:before { content: '\eabc'; }
.codicon-circle-outline:before { content: '\eabc'; }
.codicon-debug-breakpoint-unverified:before { content: '\eabc'; }
.codicon-circle-slash:before { content: '\eabd'; }
.codicon-circuit-board:before { content: '\eabe'; }
.codicon-clear-all:before { content: '\eabf'; }
.codicon-clippy:before { content: '\eac0'; }
.codicon-close-all:before { content: '\eac1'; }
.codicon-cloud-download:before { content: '\eac2'; }
.codicon-cloud-upload:before { content: '\eac3'; }
.codicon-code:before { content: '\eac4'; }
.codicon-collapse-all:before { content: '\eac5'; }
.codicon-color-mode:before { content: '\eac6'; }
.codicon-comment-discussion:before { content: '\eac7'; }
.codicon-compare-changes:before { content: '\eafd'; }
.codicon-credit-card:before { content: '\eac9'; }
.codicon-dash:before { content: '\eacc'; }
.codicon-dashboard:before { content: '\eacd'; }
.codicon-database:before { content: '\eace'; }
.codicon-debug-continue:before { content: '\eacf'; }
.codicon-debug-disconnect:before { content: '\ead0'; }
.codicon-debug-pause:before { content: '\ead1'; }
.codicon-debug-restart:before { content: '\ead2'; }
.codicon-debug-start:before { content: '\ead3'; }
.codicon-debug-step-into:before { content: '\ead4'; }
.codicon-debug-step-out:before { content: '\ead5'; }
.codicon-debug-step-over:before { content: '\ead6'; }
.codicon-debug-stop:before { content: '\ead7'; }
.codicon-debug:before { content: '\ead8'; }
.codicon-device-camera-video:before { content: '\ead9'; }
.codicon-device-camera:before { content: '\eada'; }
.codicon-device-mobile:before { content: '\eadb'; }
.codicon-diff-added:before { content: '\eadc'; }
.codicon-diff-ignored:before { content: '\eadd'; }
.codicon-diff-modified:before { content: '\eade'; }
.codicon-diff-removed:before { content: '\eadf'; }
.codicon-diff-renamed:before { content: '\eae0'; }
.codicon-diff:before { content: '\eae1'; }
.codicon-discard:before { content: '\eae2'; }
.codicon-editor-layout:before { content: '\eae3'; }
.codicon-empty-window:before { content: '\eae4'; }
.codicon-exclude:before { content: '\eae5'; }
.codicon-extensions:before { content: '\eae6'; }
.codicon-eye-closed:before { content: '\eae7'; }
.codicon-file-binary:before { content: '\eae8'; }
.codicon-file-code:before { content: '\eae9'; }
.codicon-file-media:before { content: '\eaea'; }
.codicon-file-pdf:before { content: '\eaeb'; }
.codicon-file-submodule:before { content: '\eaec'; }
.codicon-file-symlink-directory:before { content: '\eaed'; }
.codicon-file-symlink-file:before { content: '\eaee'; }
.codicon-file-zip:before { content: '\eaef'; }
.codicon-files:before { content: '\eaf0'; }
.codicon-filter:before { content: '\eaf1'; }
.codicon-flame:before { content: '\eaf2'; }
.codicon-fold-down:before { content: '\eaf3'; }
.codicon-fold-up:before { content: '\eaf4'; }
.codicon-fold:before { content: '\eaf5'; }
.codicon-folder-active:before { content: '\eaf6'; }
.codicon-folder-opened:before { content: '\eaf7'; }
.codicon-gear:before { content: '\eaf8'; }
.codicon-gift:before { content: '\eaf9'; }
.codicon-gist-secret:before { content: '\eafa'; }
.codicon-gist:before { content: '\eafb'; }
.codicon-git-commit:before { content: '\eafc'; }
.codicon-git-compare:before { content: '\eafd'; }
.codicon-git-merge:before { content: '\eafe'; }
.codicon-github-action:before { content: '\eaff'; }
.codicon-github-alt:before { content: '\eb00'; }
.codicon-globe:before { content: '\eb01'; }
.codicon-grabber:before { content: '\eb02'; }
.codicon-graph:before { content: '\eb03'; }
.codicon-gripper:before { content: '\eb04'; }
.codicon-heart:before { content: '\eb05'; }
.codicon-home:before { content: '\eb06'; }
.codicon-horizontal-rule:before { content: '\eb07'; }
.codicon-hubot:before { content: '\eb08'; }
.codicon-inbox:before { content: '\eb09'; }
.codicon-issue-closed:before { content: '\eba4'; }
.codicon-issue-reopened:before { content: '\eb0b'; }
.codicon-issues:before { content: '\eb0c'; }
.codicon-italic:before { content: '\eb0d'; }
.codicon-jersey:before { content: '\eb0e'; }
.codicon-json:before { content: '\eb0f'; }
.codicon-bracket:before { content: '\eb0f'; }
.codicon-kebab-vertical:before { content: '\eb10'; }
.codicon-key:before { content: '\eb11'; }
.codicon-law:before { content: '\eb12'; }
.codicon-lightbulb-autofix:before { content: '\eb13'; }
.codicon-link-external:before { content: '\eb14'; }
.codicon-link:before { content: '\eb15'; }
.codicon-list-ordered:before { content: '\eb16'; }
.codicon-list-unordered:before { content: '\eb17'; }
.codicon-live-share:before { content: '\eb18'; }
.codicon-loading:before { content: '\eb19'; }
.codicon-location:before { content: '\eb1a'; }
.codicon-mail-read:before { content: '\eb1b'; }
.codicon-mail:before { content: '\eb1c'; }
.codicon-markdown:before { content: '\eb1d'; }
.codicon-megaphone:before { content: '\eb1e'; }
.codicon-mention:before { content: '\eb1f'; }
.codicon-milestone:before { content: '\eb20'; }
.codicon-mortar-board:before { content: '\eb21'; }
.codicon-move:before { content: '\eb22'; }
.codicon-multiple-windows:before { content: '\eb23'; }
.codicon-mute:before { content: '\eb24'; }
.codicon-no-newline:before { content: '\eb25'; }
.codicon-note:before { content: '\eb26'; }
.codicon-octoface:before { content: '\eb27'; }
.codicon-open-preview:before { content: '\eb28'; }
.codicon-package:before { content: '\eb29'; }
.codicon-paintcan:before { content: '\eb2a'; }
.codicon-pin:before { content: '\eb2b'; }
.codicon-play:before { content: '\eb2c'; }
.codicon-run:before { content: '\eb2c'; }
.codicon-plug:before { content: '\eb2d'; }
.codicon-preserve-case:before { content: '\eb2e'; }
.codicon-preview:before { content: '\eb2f'; }
.codicon-project:before { content: '\eb30'; }
.codicon-pulse:before { content: '\eb31'; }
.codicon-question:before { content: '\eb32'; }
.codicon-quote:before { content: '\eb33'; }
.codicon-radio-tower:before { content: '\eb34'; }
.codicon-reactions:before { content: '\eb35'; }
.codicon-references:before { content: '\eb36'; }
.codicon-refresh:before { content: '\eb37'; }
.codicon-regex:before { content: '\eb38'; }
.codicon-remote-explorer:before { content: '\eb39'; }
.codicon-remote:before { content: '\eb3a'; }
.codicon-remove:before { content: '\eb3b'; }
.codicon-replace-all:before { content: '\eb3c'; }
.codicon-replace:before { content: '\eb3d'; }
.codicon-repo-clone:before { content: '\eb3e'; }
.codicon-repo-force-push:before { content: '\eb3f'; }
.codicon-repo-pull:before { content: '\eb40'; }
.codicon-repo-push:before { content: '\eb41'; }
.codicon-report:before { content: '\eb42'; }
.codicon-request-changes:before { content: '\eb43'; }
.codicon-rocket:before { content: '\eb44'; }
.codicon-root-folder-opened:before { content: '\eb45'; }
.codicon-root-folder:before { content: '\eb46'; }
.codicon-rss:before { content: '\eb47'; }
.codicon-ruby:before { content: '\eb48'; }
.codicon-save-all:before { content: '\eb49'; }
.codicon-save-as:before { content: '\eb4a'; }
.codicon-save:before { content: '\eb4b'; }
.codicon-screen-full:before { content: '\eb4c'; }
.codicon-screen-normal:before { content: '\eb4d'; }
.codicon-search-stop:before { content: '\eb4e'; }
.codicon-server:before { content: '\eb50'; }
.codicon-settings-gear:before { content: '\eb51'; }
.codicon-settings:before { content: '\eb52'; }
.codicon-shield:before { content: '\eb53'; }
.codicon-smiley:before { content: '\eb54'; }
.codicon-sort-precedence:before { content: '\eb55'; }
.codicon-split-horizontal:before { content: '\eb56'; }
.codicon-split-vertical:before { content: '\eb57'; }
.codicon-squirrel:before { content: '\eb58'; }
.codicon-star-full:before { content: '\eb59'; }
.codicon-star-half:before { content: '\eb5a'; }
.codicon-symbol-class:before { content: '\eb5b'; }
.codicon-symbol-color:before { content: '\eb5c'; }
.codicon-symbol-customcolor:before { content: '\eb5c'; }
.codicon-symbol-constant:before { content: '\eb5d'; }
.codicon-symbol-enum-member:before { content: '\eb5e'; }
.codicon-symbol-field:before { content: '\eb5f'; }
.codicon-symbol-file:before { content: '\eb60'; }
.codicon-symbol-interface:before { content: '\eb61'; }
.codicon-symbol-keyword:before { content: '\eb62'; }
.codicon-symbol-misc:before { content: '\eb63'; }
.codicon-symbol-operator:before { content: '\eb64'; }
.codicon-symbol-property:before { content: '\eb65'; }
.codicon-wrench:before { content: '\eb65'; }
.codicon-wrench-subaction:before { content: '\eb65'; }
.codicon-symbol-snippet:before { content: '\eb66'; }
.codicon-tasklist:before { content: '\eb67'; }
.codicon-telescope:before { content: '\eb68'; }
.codicon-text-size:before { content: '\eb69'; }
.codicon-three-bars:before { content: '\eb6a'; }
.codicon-thumbsdown:before { content: '\eb6b'; }
.codicon-thumbsup:before { content: '\eb6c'; }
.codicon-tools:before { content: '\eb6d'; }
.codicon-triangle-down:before { content: '\eb6e'; }
.codicon-triangle-left:before { content: '\eb6f'; }
.codicon-triangle-right:before { content: '\eb70'; }
.codicon-triangle-up:before { content: '\eb71'; }
.codicon-twitter:before { content: '\eb72'; }
.codicon-unfold:before { content: '\eb73'; }
.codicon-unlock:before { content: '\eb74'; }
.codicon-unmute:before { content: '\eb75'; }
.codicon-unverified:before { content: '\eb76'; }
.codicon-verified:before { content: '\eb77'; }
.codicon-versions:before { content: '\eb78'; }
.codicon-vm-active:before { content: '\eb79'; }
.codicon-vm-outline:before { content: '\eb7a'; }
.codicon-vm-running:before { content: '\eb7b'; }
.codicon-watch:before { content: '\eb7c'; }
.codicon-whitespace:before { content: '\eb7d'; }
.codicon-whole-word:before { content: '\eb7e'; }
.codicon-window:before { content: '\eb7f'; }
.codicon-word-wrap:before { content: '\eb80'; }
.codicon-zoom-in:before { content: '\eb81'; }
.codicon-zoom-out:before { content: '\eb82'; }
.codicon-list-filter:before { content: '\eb83'; }
.codicon-list-flat:before { content: '\eb84'; }
.codicon-list-selection:before { content: '\eb85'; }
.codicon-selection:before { content: '\eb85'; }
.codicon-list-tree:before { content: '\eb86'; }
.codicon-debug-breakpoint-function-unverified:before { content: '\eb87'; }
.codicon-debug-breakpoint-function:before { content: '\eb88'; }
.codicon-debug-breakpoint-function-disabled:before { content: '\eb88'; }
.codicon-debug-stackframe-active:before { content: '\eb89'; }
.codicon-circle-small-filled:before { content: '\eb8a'; }
.codicon-debug-stackframe-dot:before { content: '\eb8a'; }
.codicon-debug-stackframe:before { content: '\eb8b'; }
.codicon-debug-stackframe-focused:before { content: '\eb8b'; }
.codicon-debug-breakpoint-unsupported:before { content: '\eb8c'; }
.codicon-symbol-string:before { content: '\eb8d'; }
.codicon-debug-reverse-continue:before { content: '\eb8e'; }
.codicon-debug-step-back:before { content: '\eb8f'; }
.codicon-debug-restart-frame:before { content: '\eb90'; }
.codicon-call-incoming:before { content: '\eb92'; }
.codicon-call-outgoing:before { content: '\eb93'; }
.codicon-menu:before { content: '\eb94'; }
.codicon-expand-all:before { content: '\eb95'; }
.codicon-feedback:before { content: '\eb96'; }
.codicon-group-by-ref-type:before { content: '\eb97'; }
.codicon-ungroup-by-ref-type:before { content: '\eb98'; }
.codicon-account:before { content: '\eb99'; }
.codicon-bell-dot:before { content: '\eb9a'; }
.codicon-debug-console:before { content: '\eb9b'; }
.codicon-library:before { content: '\eb9c'; }
.codicon-output:before { content: '\eb9d'; }
.codicon-run-all:before { content: '\eb9e'; }
.codicon-sync-ignored:before { content: '\eb9f'; }
.codicon-pinned:before { content: '\eba0'; }
.codicon-github-inverted:before { content: '\eba1'; }
.codicon-debug-alt:before { content: '\eb91'; }
.codicon-server-process:before { content: '\eba2'; }
.codicon-server-environment:before { content: '\eba3'; }
.codicon-pass:before { content: '\eba4'; }
.codicon-stop-circle:before { content: '\eba5'; }
.codicon-play-circle:before { content: '\eba6'; }
.codicon-record:before { content: '\eba7'; }
.codicon-debug-alt-small:before { content: '\eba8'; }
.codicon-vm-connect:before { content: '\eba9'; }
.codicon-cloud:before { content: '\ebaa'; }
.codicon-merge:before { content: '\ebab'; }
.codicon-export:before { content: '\ebac'; }
.codicon-graph-left:before { content: '\ebad'; }
.codicon-magnet:before { content: '\ebae'; }
.codicon-notebook:before { content: '\ebaf'; }
.codicon-redo:before { content: '\ebb0'; }
.codicon-check-all:before { content: '\ebb1'; }
.codicon-pinned-dirty:before { content: '\ebb2'; }
.codicon-pass-filled:before { content: '\ebb3'; }
.codicon-circle-large-filled:before { content: '\ebb4'; }
.codicon-circle-large:before { content: '\ebb5'; }
.codicon-circle-large-outline:before { content: '\ebb5'; }
.codicon-combine:before { content: '\ebb6'; }
.codicon-gather:before { content: '\ebb6'; }
.codicon-table:before { content: '\ebb7'; }
.codicon-variable-group:before { content: '\ebb8'; }
.codicon-type-hierarchy:before { content: '\ebb9'; }
.codicon-type-hierarchy-sub:before { content: '\ebba'; }
.codicon-type-hierarchy-super:before { content: '\ebbb'; }
.codicon-git-pull-request-create:before { content: '\ebbc'; }
.codicon-run-above:before { content: '\ebbd'; }
.codicon-run-below:before { content: '\ebbe'; }
.codicon-notebook-template:before { content: '\ebbf'; }
.codicon-debug-rerun:before { content: '\ebc0'; }
.codicon-workspace-trusted:before { content: '\ebc1'; }
.codicon-workspace-untrusted:before { content: '\ebc2'; }
.codicon-workspace-unspecified:before { content: '\ebc3'; }
.codicon-terminal-cmd:before { content: '\ebc4'; }
.codicon-terminal-debian:before { content: '\ebc5'; }
.codicon-terminal-linux:before { content: '\ebc6'; }
.codicon-terminal-powershell:before { content: '\ebc7'; }
.codicon-terminal-tmux:before { content: '\ebc8'; }
.codicon-terminal-ubuntu:before { content: '\ebc9'; }
.codicon-terminal-bash:before { content: '\ebca'; }
.codicon-arrow-swap:before { content: '\ebcb'; }
.codicon-copy:before { content: '\ebcc'; }
.codicon-person-add:before { content: '\ebcd'; }
.codicon-filter-filled:before { content: '\ebce'; }
.codicon-wand:before { content: '\ebcf'; }
.codicon-debug-line-by-line:before { content: '\ebd0'; }
.codicon-inspect:before { content: '\ebd1'; }
.codicon-layers:before { content: '\ebd2'; }
.codicon-layers-dot:before { content: '\ebd3'; }
.codicon-layers-active:before { content: '\ebd4'; }
.codicon-compass:before { content: '\ebd5'; }
.codicon-compass-dot:before { content: '\ebd6'; }
.codicon-compass-active:before { content: '\ebd7'; }
.codicon-azure:before { content: '\ebd8'; }
.codicon-issue-draft:before { content: '\ebd9'; }
.codicon-git-pull-request-closed:before { content: '\ebda'; }
.codicon-git-pull-request-draft:before { content: '\ebdb'; }
.codicon-debug-all:before { content: '\ebdc'; }
.codicon-debug-coverage:before { content: '\ebdd'; }
.codicon-run-errors:before { content: '\ebde'; }
.codicon-folder-library:before { content: '\ebdf'; }
.codicon-debug-continue-small:before { content: '\ebe0'; }
.codicon-beaker-stop:before { content: '\ebe1'; }
.codicon-graph-line:before { content: '\ebe2'; }
.codicon-graph-scatter:before { content: '\ebe3'; }
.codicon-pie-chart:before { content: '\ebe4'; }
.codicon-bracket-dot:before { content: '\ebe5'; }
.codicon-bracket-error:before { content: '\ebe6'; }
.codicon-lock-small:before { content: '\ebe7'; }
.codicon-azure-devops:before { content: '\ebe8'; }
.codicon-verified-filled:before { content: '\ebe9'; }
.codicon-newline:before { content: '\ebea'; }
.codicon-layout:before { content: '\ebeb'; }
.codicon-layout-activitybar-left:before { content: '\ebec'; }
.codicon-layout-activitybar-right:before { content: '\ebed'; }
.codicon-layout-panel-left:before { content: '\ebee'; }
.codicon-layout-panel-center:before { content: '\ebef'; }
.codicon-layout-panel-justify:before { content: '\ebf0'; }
.codicon-layout-panel-right:before { content: '\ebf1'; }
.codicon-layout-panel:before { content: '\ebf2'; }
.codicon-layout-sidebar-left:before { content: '\ebf3'; }
.codicon-layout-sidebar-right:before { content: '\ebf4'; }
.codicon-layout-statusbar:before { content: '\ebf5'; }
.codicon-layout-menubar:before { content: '\ebf6'; }
.codicon-layout-centered:before { content: '\ebf7'; }
.codicon-layout-sidebar-right-off:before { content: '\ec00'; }
.codicon-layout-panel-off:before { content: '\ec01'; }
.codicon-layout-sidebar-left-off:before { content: '\ec02'; }
.codicon-target:before { content: '\ebf8'; }
.codicon-indent:before { content: '\ebf9'; }
.codicon-record-small:before { content: '\ebfa'; }
.codicon-error-small:before { content: '\ebfb'; }
.codicon-arrow-circle-down:before { content: '\ebfc'; }
.codicon-arrow-circle-left:before { content: '\ebfd'; }
.codicon-arrow-circle-right:before { content: '\ebfe'; }
.codicon-arrow-circle-up:before { content: '\ebff'; }
.codicon-heart-filled:before { content: '\ec04'; }
.codicon-map:before { content: '\ec05'; }
.codicon-map-filled:before { content: '\ec06'; }
.codicon-circle-small:before { content: '\ec07'; }
.codicon-bell-slash:before { content: '\ec08'; }
.codicon-bell-slash-dot:before { content: '\ec09'; }
.codicon-comment-unresolved:before { content: '\ec0a'; }
.codicon-git-pull-request-go-to-changes:before { content: '\ec0b'; }
.codicon-git-pull-request-new-changes:before { content: '\ec0c'; }
.codicon-search-fuzzy:before { content: '\ec0d'; }
.codicon-comment-draft:before { content: '\ec0e'; }
.codicon-send:before { content: '\ec0f'; }
.codicon-sparkle:before { content: '\ec10'; }
.codicon-insert:before { content: '\ec11'; }
.codicon-dialog-error:before { content: '\ea87'; }
.codicon-dialog-warning:before { content: '\ea6c'; }
.codicon-dialog-info:before { content: '\ea74'; }
.codicon-dialog-close:before { content: '\ea76'; }
.codicon-tree-item-expanded:before { content: '\eab4'; }
.codicon-tree-filter-on-type-on:before { content: '\eb83'; }
.codicon-tree-filter-on-type-off:before { content: '\eb85'; }
.codicon-tree-filter-clear:before { content: '\ea76'; }
.codicon-tree-item-loading:before { content: '\eb19'; }
.codicon-menu-selection:before { content: '\eab2'; }
.codicon-menu-submenu:before { content: '\eab6'; }
.codicon-menubar-more:before { content: '\ea7c'; }
.codicon-scrollbar-button-left:before { content: '\eb6f'; }
.codicon-scrollbar-button-right:before { content: '\eb70'; }
.codicon-scrollbar-button-up:before { content: '\eb71'; }
.codicon-scrollbar-button-down:before { content: '\eb6e'; }
.codicon-toolbar-more:before { content: '\ea7c'; }
.codicon-quick-input-back:before { content: '\ea9b'; }
.codicon-widget-close:before { content: '\ea76'; }
.codicon-goto-previous-location:before { content: '\eaa1'; }
.codicon-goto-next-location:before { content: '\ea9a'; }
.codicon-diff-review-insert:before { content: '\ea60'; }
.codicon-diff-review-remove:before { content: '\eb3b'; }
.codicon-diff-review-close:before { content: '\ea76'; }
.codicon-parameter-hints-next:before { content: '\eab4'; }
.codicon-parameter-hints-previous:before { content: '\eab7'; }
.codicon-suggest-more-info:before { content: '\eab6'; }
.codicon-inline-suggestion-hints-next:before { content: '\eab6'; }
.codicon-inline-suggestion-hints-previous:before { content: '\eab5'; }
.codicon-diff-insert:before { content: '\ea60'; }
.codicon-diff-remove:before { content: '\eb3b'; }
.codicon-find-selection:before { content: '\eb85'; }
.codicon-find-collapsed:before { content: '\eab6'; }
.codicon-find-expanded:before { content: '\eab4'; }
.codicon-find-replace:before { content: '\eb3d'; }
.codicon-find-replace-all:before { content: '\eb3c'; }
.codicon-find-previous-match:before { content: '\eaa1'; }
.codicon-find-next-match:before { content: '\ea9a'; }
.codicon-folding-expanded:before { content: '\eab4'; }
.codicon-folding-collapsed:before { content: '\eab6'; }
.codicon-folding-manual-collapsed:before { content: '\eab6'; }
.codicon-folding-manual-expanded:before { content: '\eab4'; }
.codicon-marker-navigation-next:before { content: '\ea9a'; }
.codicon-marker-navigation-previous:before { content: '\eaa1'; }
.codicon-extensions-warning-message:before { content: '\ea6c'; }
.monaco-editor .inputarea.ime-input { background-color: #1e1e1e; }
.monaco-editor .view-overlays .current-line { border: 2px solid #282828; }
.monaco-editor .margin-view-overlays .current-line-margin { border: 2px solid #282828; }
.monaco-editor .bracket-indent-guide.lvl-0 { --guide-color: rgba(255, 215, 0, 0.3); --guide-color-active: #ffd700; }
.monaco-editor .bracket-indent-guide.lvl-1 { --guide-color: rgba(218, 112, 214, 0.3); --guide-color-active: #da70d6; }
.monaco-editor .bracket-indent-guide.lvl-2 { --guide-color: rgba(23, 159, 255, 0.3); --guide-color-active: #179fff; }
.monaco-editor .bracket-indent-guide.lvl-3 { --guide-color: rgba(255, 215, 0, 0.3); --guide-color-active: #ffd700; }
.monaco-editor .bracket-indent-guide.lvl-4 { --guide-color: rgba(218, 112, 214, 0.3); --guide-color-active: #da70d6; }
.monaco-editor .bracket-indent-guide.lvl-5 { --guide-color: rgba(23, 159, 255, 0.3); --guide-color-active: #179fff; }
.monaco-editor .bracket-indent-guide.lvl-6 { --guide-color: rgba(255, 215, 0, 0.3); --guide-color-active: #ffd700; }
.monaco-editor .bracket-indent-guide.lvl-7 { --guide-color: rgba(218, 112, 214, 0.3); --guide-color-active: #da70d6; }
.monaco-editor .bracket-indent-guide.lvl-8 { --guide-color: rgba(23, 159, 255, 0.3); --guide-color-active: #179fff; }
.monaco-editor .bracket-indent-guide.lvl-9 { --guide-color: rgba(255, 215, 0, 0.3); --guide-color-active: #ffd700; }
.monaco-editor .bracket-indent-guide.lvl-10 { --guide-color: rgba(218, 112, 214, 0.3); --guide-color-active: #da70d6; }
.monaco-editor .bracket-indent-guide.lvl-11 { --guide-color: rgba(23, 159, 255, 0.3); --guide-color-active: #179fff; }
.monaco-editor .bracket-indent-guide.lvl-12 { --guide-color: rgba(255, 215, 0, 0.3); --guide-color-active: #ffd700; }
.monaco-editor .bracket-indent-guide.lvl-13 { --guide-color: rgba(218, 112, 214, 0.3); --guide-color-active: #da70d6; }
.monaco-editor .bracket-indent-guide.lvl-14 { --guide-color: rgba(23, 159, 255, 0.3); --guide-color-active: #179fff; }
.monaco-editor .bracket-indent-guide.lvl-15 { --guide-color: rgba(255, 215, 0, 0.3); --guide-color-active: #ffd700; }
.monaco-editor .bracket-indent-guide.lvl-16 { --guide-color: rgba(218, 112, 214, 0.3); --guide-color-active: #da70d6; }
.monaco-editor .bracket-indent-guide.lvl-17 { --guide-color: rgba(23, 159, 255, 0.3); --guide-color-active: #179fff; }
.monaco-editor .bracket-indent-guide.lvl-18 { --guide-color: rgba(255, 215, 0, 0.3); --guide-color-active: #ffd700; }
.monaco-editor .bracket-indent-guide.lvl-19 { --guide-color: rgba(218, 112, 214, 0.3); --guide-color-active: #da70d6; }
.monaco-editor .bracket-indent-guide.lvl-20 { --guide-color: rgba(23, 159, 255, 0.3); --guide-color-active: #179fff; }
.monaco-editor .bracket-indent-guide.lvl-21 { --guide-color: rgba(255, 215, 0, 0.3); --guide-color-active: #ffd700; }
.monaco-editor .bracket-indent-guide.lvl-22 { --guide-color: rgba(218, 112, 214, 0.3); --guide-color-active: #da70d6; }
.monaco-editor .bracket-indent-guide.lvl-23 { --guide-color: rgba(23, 159, 255, 0.3); --guide-color-active: #179fff; }
.monaco-editor .bracket-indent-guide.lvl-24 { --guide-color: rgba(255, 215, 0, 0.3); --guide-color-active: #ffd700; }
.monaco-editor .bracket-indent-guide.lvl-25 { --guide-color: rgba(218, 112, 214, 0.3); --guide-color-active: #da70d6; }
.monaco-editor .bracket-indent-guide.lvl-26 { --guide-color: rgba(23, 159, 255, 0.3); --guide-color-active: #179fff; }
.monaco-editor .bracket-indent-guide.lvl-27 { --guide-color: rgba(255, 215, 0, 0.3); --guide-color-active: #ffd700; }
.monaco-editor .bracket-indent-guide.lvl-28 { --guide-color: rgba(218, 112, 214, 0.3); --guide-color-active: #da70d6; }
.monaco-editor .bracket-indent-guide.lvl-29 { --guide-color: rgba(23, 159, 255, 0.3); --guide-color-active: #179fff; }
.monaco-editor .vertical { box-shadow: 1px 0 0 0 var(--guide-color) inset; }
.monaco-editor .horizontal-top { border-top: 1px solid var(--guide-color); }
.monaco-editor .horizontal-bottom { border-bottom: 1px solid var(--guide-color); }
.monaco-editor .vertical.indent-active { box-shadow: 1px 0 0 0 var(--guide-color-active) inset; }
.monaco-editor .horizontal-top.indent-active { border-top: 1px solid var(--guide-color-active); }
.monaco-editor .horizontal-bottom.indent-active { border-bottom: 1px solid var(--guide-color-active); }
.monaco-editor .line-numbers.dimmed-line-number { color: rgba(133, 133, 133, 0.4); }
.monaco-editor .cursors-layer .cursor { background-color: #aeafad; border-color: #aeafad; color: #515052; }
.monaco-editor .unexpected-closing-bracket { color: rgba(255, 18, 18, 0.8); }
.monaco-editor .bracket-highlighting-0 { color: #ffd700; }
.monaco-editor .bracket-highlighting-1 { color: #da70d6; }
.monaco-editor .bracket-highlighting-2 { color: #179fff; }
.monaco-editor .bracket-highlighting-3 { color: #ffd700; }
.monaco-editor .bracket-highlighting-4 { color: #da70d6; }
.monaco-editor .bracket-highlighting-5 { color: #179fff; }
.monaco-editor .bracket-highlighting-6 { color: #ffd700; }
.monaco-editor .bracket-highlighting-7 { color: #da70d6; }
.monaco-editor .bracket-highlighting-8 { color: #179fff; }
.monaco-editor .bracket-highlighting-9 { color: #ffd700; }
.monaco-editor .bracket-highlighting-10 { color: #da70d6; }
.monaco-editor .bracket-highlighting-11 { color: #179fff; }
.monaco-editor .bracket-highlighting-12 { color: #ffd700; }
.monaco-editor .bracket-highlighting-13 { color: #da70d6; }
.monaco-editor .bracket-highlighting-14 { color: #179fff; }
.monaco-editor .bracket-highlighting-15 { color: #ffd700; }
.monaco-editor .bracket-highlighting-16 { color: #da70d6; }
.monaco-editor .bracket-highlighting-17 { color: #179fff; }
.monaco-editor .bracket-highlighting-18 { color: #ffd700; }
.monaco-editor .bracket-highlighting-19 { color: #da70d6; }
.monaco-editor .bracket-highlighting-20 { color: #179fff; }
.monaco-editor .bracket-highlighting-21 { color: #ffd700; }
.monaco-editor .bracket-highlighting-22 { color: #da70d6; }
.monaco-editor .bracket-highlighting-23 { color: #179fff; }
.monaco-editor .bracket-highlighting-24 { color: #ffd700; }
.monaco-editor .bracket-highlighting-25 { color: #da70d6; }
.monaco-editor .bracket-highlighting-26 { color: #179fff; }
.monaco-editor .bracket-highlighting-27 { color: #ffd700; }
.monaco-editor .bracket-highlighting-28 { color: #da70d6; }
.monaco-editor .bracket-highlighting-29 { color: #179fff; }
.monaco-editor .squiggly-error { background: url("data:image/svg+xml,%3Csvg%20xmlns%3D'http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg'%20viewBox%3D'0%200%206%203'%20enable-background%3D'new%200%200%206%203'%20height%3D'3'%20width%3D'6'%3E%3Cg%20fill%3D'%23f14c4c'%3E%3Cpolygon%20points%3D'5.5%2C0%202.5%2C3%201.1%2C3%204.1%2C0'%2F%3E%3Cpolygon%20points%3D'4%2C0%206%2C2%206%2C0.6%205.4%2C0'%2F%3E%3Cpolygon%20points%3D'0%2C2%201%2C3%202.4%2C3%200%2C0.6'%2F%3E%3C%2Fg%3E%3C%2Fsvg%3E") repeat-x bottom left; }
.monaco-editor .squiggly-warning { background: url("data:image/svg+xml,%3Csvg%20xmlns%3D'http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg'%20viewBox%3D'0%200%206%203'%20enable-background%3D'new%200%200%206%203'%20height%3D'3'%20width%3D'6'%3E%3Cg%20fill%3D'%23cca700'%3E%3Cpolygon%20points%3D'5.5%2C0%202.5%2C3%201.1%2C3%204.1%2C0'%2F%3E%3Cpolygon%20points%3D'4%2C0%206%2C2%206%2C0.6%205.4%2C0'%2F%3E%3Cpolygon%20points%3D'0%2C2%201%2C3%202.4%2C3%200%2C0.6'%2F%3E%3C%2Fg%3E%3C%2Fsvg%3E") repeat-x bottom left; }
.monaco-editor .squiggly-info { background: url("data:image/svg+xml,%3Csvg%20xmlns%3D'http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg'%20viewBox%3D'0%200%206%203'%20enable-background%3D'new%200%200%206%203'%20height%3D'3'%20width%3D'6'%3E%3Cg%20fill%3D'%233794ff'%3E%3Cpolygon%20points%3D'5.5%2C0%202.5%2C3%201.1%2C3%204.1%2C0'%2F%3E%3Cpolygon%20points%3D'4%2C0%206%2C2%206%2C0.6%205.4%2C0'%2F%3E%3Cpolygon%20points%3D'0%2C2%201%2C3%202.4%2C3%200%2C0.6'%2F%3E%3C%2Fg%3E%3C%2Fsvg%3E") repeat-x bottom left; }
.monaco-editor .squiggly-hint { background: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20height%3D%223%22%20width%3D%2212%22%3E%3Cg%20fill%3D%22rgba(238%2C%20238%2C%20238%2C%200.7)%22%3E%3Ccircle%20cx%3D%221%22%20cy%3D%221%22%20r%3D%221%22%2F%3E%3Ccircle%20cx%3D%225%22%20cy%3D%221%22%20r%3D%221%22%2F%3E%3Ccircle%20cx%3D%229%22%20cy%3D%221%22%20r%3D%221%22%2F%3E%3C%2Fg%3E%3C%2Fsvg%3E") no-repeat bottom left; }
.monaco-editor.showUnused .squiggly-inline-unnecessary { opacity: 0.667; }
.monaco-editor .selectionHighlight { background-color: rgba(173, 214, 255, 0.07); }

	.monaco-editor .diagonal-fill {
		background-image: linear-gradient(
			-45deg,
			rgba(204, 204, 204, 0.2) 12.5%,
			#0000 12.5%, #0000 50%,
			rgba(204, 204, 204, 0.2) 50%, rgba(204, 204, 204, 0.2) 62.5%,
			#0000 62.5%, #0000 100%
		);
		background-size: 8px 8px;
	}
	
.monaco-editor .findMatch { background-color: rgba(234, 92, 0, 0.33); }
.monaco-editor .currentFindMatch { background-color: #515c6a; }
.monaco-editor .findScope { background-color: rgba(58, 61, 65, 0.4); }
.monaco-editor .find-widget { background-color: #252526; }
.monaco-editor .find-widget { box-shadow: 0 0 8px 2px rgba(0, 0, 0, 0.36); }
.monaco-editor .find-widget { color: #cccccc; }
.monaco-editor .find-widget.no-results .matchesCount { color: #f48771; }
.monaco-editor .find-widget .monaco-sash { background-color: #454545; }

		.monaco-editor .find-widget .button:not(.disabled):hover,
		.monaco-editor .find-widget .codicon-find-selection:hover {
			background-color: rgba(90, 93, 94, 0.31) !important;
		}
	
.monaco-editor .find-widget .monaco-inputbox.synthetic-focus { outline-color: #007fd4; }
.monaco-editor .monaco-hover .hover-row:not(:first-child):not(:empty) { border-top: 1px solid rgba(69, 69, 69, 0.5); }
.monaco-editor .monaco-hover hr { border-top: 1px solid rgba(69, 69, 69, 0.5); }
.monaco-editor .monaco-hover hr { border-bottom: 0px solid rgba(69, 69, 69, 0.5); }
.monaco-editor { --vscode-foreground: #cccccc;
--vscode-disabledForeground: rgba(204, 204, 204, 0.5);
--vscode-errorForeground: #f48771;
--vscode-descriptionForeground: rgba(204, 204, 204, 0.7);
--vscode-icon-foreground: #c5c5c5;
--vscode-focusBorder: #007fd4;
--vscode-textSeparator-foreground: rgba(255, 255, 255, 0.18);
--vscode-textLink-foreground: #3794ff;
--vscode-textLink-activeForeground: #3794ff;
--vscode-textPreformat-foreground: #d7ba7d;
--vscode-textBlockQuote-background: rgba(127, 127, 127, 0.1);
--vscode-textBlockQuote-border: rgba(0, 122, 204, 0.5);
--vscode-textCodeBlock-background: rgba(10, 10, 10, 0.4);
--vscode-widget-shadow: rgba(0, 0, 0, 0.36);
--vscode-input-background: #3c3c3c;
--vscode-input-foreground: #cccccc;
--vscode-inputOption-activeBorder: #007acc;
--vscode-inputOption-hoverBackground: rgba(90, 93, 94, 0.5);
--vscode-inputOption-activeBackground: rgba(0, 127, 212, 0.4);
--vscode-inputOption-activeForeground: #ffffff;
--vscode-input-placeholderForeground: rgba(204, 204, 204, 0.5);
--vscode-inputValidation-infoBackground: #063b49;
--vscode-inputValidation-infoBorder: #007acc;
--vscode-inputValidation-warningBackground: #352a05;
--vscode-inputValidation-warningBorder: #b89500;
--vscode-inputValidation-errorBackground: #5a1d1d;
--vscode-inputValidation-errorBorder: #be1100;
--vscode-dropdown-background: #3c3c3c;
--vscode-dropdown-foreground: #f0f0f0;
--vscode-dropdown-border: #3c3c3c;
--vscode-button-foreground: #ffffff;
--vscode-button-separator: rgba(255, 255, 255, 0.4);
--vscode-button-background: #0e639c;
--vscode-button-hoverBackground: #1177bb;
--vscode-button-secondaryForeground: #ffffff;
--vscode-button-secondaryBackground: #3a3d41;
--vscode-button-secondaryHoverBackground: #45494e;
--vscode-badge-background: #4d4d4d;
--vscode-badge-foreground: #ffffff;
--vscode-scrollbar-shadow: #000000;
--vscode-scrollbarSlider-background: rgba(121, 121, 121, 0.4);
--vscode-scrollbarSlider-hoverBackground: rgba(100, 100, 100, 0.7);
--vscode-scrollbarSlider-activeBackground: rgba(191, 191, 191, 0.4);
--vscode-progressBar-background: #0e70c0;
--vscode-editorError-foreground: #f14c4c;
--vscode-editorWarning-foreground: #cca700;
--vscode-editorInfo-foreground: #3794ff;
--vscode-editorHint-foreground: rgba(238, 238, 238, 0.7);
--vscode-sash-hoverBorder: #007fd4;
--vscode-editor-background: #1e1e1e;
--vscode-editor-foreground: #d4d4d4;
--vscode-editorStickyScroll-background: #1e1e1e;
--vscode-editorStickyScrollHover-background: #2a2d2e;
--vscode-editorWidget-background: #252526;
--vscode-editorWidget-foreground: #cccccc;
--vscode-editorWidget-border: #454545;
--vscode-quickInput-background: #252526;
--vscode-quickInput-foreground: #cccccc;
--vscode-quickInputTitle-background: rgba(255, 255, 255, 0.1);
--vscode-pickerGroup-foreground: #3794ff;
--vscode-pickerGroup-border: #3f3f46;
--vscode-keybindingLabel-background: rgba(128, 128, 128, 0.17);
--vscode-keybindingLabel-foreground: #cccccc;
--vscode-keybindingLabel-border: rgba(51, 51, 51, 0.6);
--vscode-keybindingLabel-bottomBorder: rgba(68, 68, 68, 0.6);
--vscode-editor-selectionBackground: #264f78;
--vscode-editor-inactiveSelectionBackground: #3a3d41;
--vscode-editor-selectionHighlightBackground: rgba(173, 214, 255, 0.15);
--vscode-editor-findMatchBackground: #515c6a;
--vscode-editor-findMatchHighlightBackground: rgba(234, 92, 0, 0.33);
--vscode-editor-findRangeHighlightBackground: rgba(58, 61, 65, 0.4);
--vscode-searchEditor-findMatchBackground: rgba(234, 92, 0, 0.22);
--vscode-search-resultsInfoForeground: rgba(204, 204, 204, 0.65);
--vscode-editor-hoverHighlightBackground: rgba(38, 79, 120, 0.25);
--vscode-editorHoverWidget-background: #252526;
--vscode-editorHoverWidget-foreground: #cccccc;
--vscode-editorHoverWidget-border: #454545;
--vscode-editorHoverWidget-statusBarBackground: #2c2c2d;
--vscode-editorLink-activeForeground: #4e94ce;
--vscode-editorInlayHint-foreground: #cccccc;
--vscode-editorInlayHint-background: rgba(77, 77, 77, 0.25);
--vscode-editorInlayHint-typeForeground: #cccccc;
--vscode-editorInlayHint-typeBackground: rgba(77, 77, 77, 0.25);
--vscode-editorInlayHint-parameterForeground: #cccccc;
--vscode-editorInlayHint-parameterBackground: rgba(77, 77, 77, 0.25);
--vscode-editorLightBulb-foreground: #ffcc00;
--vscode-editorLightBulbAutoFix-foreground: #75beff;
--vscode-diffEditor-insertedTextBackground: rgba(156, 204, 44, 0.13);
--vscode-diffEditor-removedTextBackground: rgba(255, 0, 0, 0.14);
--vscode-diffEditor-insertedLineBackground: rgba(156, 204, 44, 0.13);
--vscode-diffEditor-removedLineBackground: rgba(255, 0, 0, 0.14);
--vscode-diffEditor-diagonalFill: rgba(204, 204, 204, 0.2);
--vscode-diffEditor-unchangedRegionBackground: #3e3e3e;
--vscode-diffEditor-unchangedRegionForeground: #a3a2a2;
--vscode-diffEditor-unchangedCodeBackground: rgba(116, 116, 116, 0.16);
--vscode-list-focusOutline: #007fd4;
--vscode-list-activeSelectionBackground: #04395e;
--vscode-list-activeSelectionForeground: #ffffff;
--vscode-list-inactiveSelectionBackground: #37373d;
--vscode-list-hoverBackground: #2a2d2e;
--vscode-list-dropBackground: #062f4a;
--vscode-list-highlightForeground: #2aaaff;
--vscode-list-focusHighlightForeground: #2aaaff;
--vscode-list-invalidItemForeground: #b89500;
--vscode-list-errorForeground: #f88070;
--vscode-list-warningForeground: #cca700;
--vscode-listFilterWidget-background: #252526;
--vscode-listFilterWidget-outline: rgba(0, 0, 0, 0);
--vscode-listFilterWidget-noMatchesOutline: #be1100;
--vscode-listFilterWidget-shadow: rgba(0, 0, 0, 0.36);
--vscode-list-filterMatchBackground: rgba(234, 92, 0, 0.33);
--vscode-tree-indentGuidesStroke: #585858;
--vscode-tree-inactiveIndentGuidesStroke: rgba(88, 88, 88, 0.4);
--vscode-tree-tableColumnsBorder: rgba(204, 204, 204, 0.13);
--vscode-tree-tableOddRowsBackground: rgba(204, 204, 204, 0.04);
--vscode-list-deemphasizedForeground: #8c8c8c;
--vscode-checkbox-background: #3c3c3c;
--vscode-checkbox-selectBackground: #252526;
--vscode-checkbox-foreground: #f0f0f0;
--vscode-checkbox-border: #3c3c3c;
--vscode-checkbox-selectBorder: #c5c5c5;
--vscode-quickInputList-focusForeground: #ffffff;
--vscode-quickInputList-focusBackground: #04395e;
--vscode-menu-foreground: #f0f0f0;
--vscode-menu-background: #3c3c3c;
--vscode-menu-selectionForeground: #ffffff;
--vscode-menu-selectionBackground: #04395e;
--vscode-menu-separatorBackground: #606060;
--vscode-toolbar-hoverBackground: rgba(90, 93, 94, 0.31);
--vscode-toolbar-activeBackground: rgba(99, 102, 103, 0.31);
--vscode-editor-snippetTabstopHighlightBackground: rgba(124, 124, 124, 0.3);
--vscode-editor-snippetFinalTabstopHighlightBorder: #525252;
--vscode-breadcrumb-foreground: rgba(204, 204, 204, 0.8);
--vscode-breadcrumb-background: #1e1e1e;
--vscode-breadcrumb-focusForeground: #e0e0e0;
--vscode-breadcrumb-activeSelectionForeground: #e0e0e0;
--vscode-breadcrumbPicker-background: #252526;
--vscode-merge-currentHeaderBackground: rgba(64, 200, 174, 0.5);
--vscode-merge-currentContentBackground: rgba(64, 200, 174, 0.2);
--vscode-merge-incomingHeaderBackground: rgba(64, 166, 255, 0.5);
--vscode-merge-incomingContentBackground: rgba(64, 166, 255, 0.2);
--vscode-merge-commonHeaderBackground: rgba(96, 96, 96, 0.4);
--vscode-merge-commonContentBackground: rgba(96, 96, 96, 0.16);
--vscode-editorOverviewRuler-currentContentForeground: rgba(64, 200, 174, 0.5);
--vscode-editorOverviewRuler-incomingContentForeground: rgba(64, 166, 255, 0.5);
--vscode-editorOverviewRuler-commonContentForeground: rgba(96, 96, 96, 0.4);
--vscode-editorOverviewRuler-findMatchForeground: rgba(209, 134, 22, 0.49);
--vscode-editorOverviewRuler-selectionHighlightForeground: rgba(160, 160, 160, 0.8);
--vscode-minimap-findMatchHighlight: #d18616;
--vscode-minimap-selectionOccurrenceHighlight: #676767;
--vscode-minimap-selectionHighlight: #264f78;
--vscode-minimap-errorHighlight: rgba(255, 18, 18, 0.7);
--vscode-minimap-warningHighlight: #cca700;
--vscode-minimap-foregroundOpacity: #000000;
--vscode-minimapSlider-background: rgba(121, 121, 121, 0.2);
--vscode-minimapSlider-hoverBackground: rgba(100, 100, 100, 0.35);
--vscode-minimapSlider-activeBackground: rgba(191, 191, 191, 0.2);
--vscode-problemsErrorIcon-foreground: #f14c4c;
--vscode-problemsWarningIcon-foreground: #cca700;
--vscode-problemsInfoIcon-foreground: #3794ff;
--vscode-charts-foreground: #cccccc;
--vscode-charts-lines: rgba(204, 204, 204, 0.5);
--vscode-charts-red: #f14c4c;
--vscode-charts-blue: #3794ff;
--vscode-charts-yellow: #cca700;
--vscode-charts-orange: #d18616;
--vscode-charts-green: #89d185;
--vscode-charts-purple: #b180d7;
--vscode-symbolIcon-arrayForeground: #cccccc;
--vscode-symbolIcon-booleanForeground: #cccccc;
--vscode-symbolIcon-classForeground: #ee9d28;
--vscode-symbolIcon-colorForeground: #cccccc;
--vscode-symbolIcon-constantForeground: #cccccc;
--vscode-symbolIcon-constructorForeground: #b180d7;
--vscode-symbolIcon-enumeratorForeground: #ee9d28;
--vscode-symbolIcon-enumeratorMemberForeground: #75beff;
--vscode-symbolIcon-eventForeground: #ee9d28;
--vscode-symbolIcon-fieldForeground: #75beff;
--vscode-symbolIcon-fileForeground: #cccccc;
--vscode-symbolIcon-folderForeground: #cccccc;
--vscode-symbolIcon-functionForeground: #b180d7;
--vscode-symbolIcon-interfaceForeground: #75beff;
--vscode-symbolIcon-keyForeground: #cccccc;
--vscode-symbolIcon-keywordForeground: #cccccc;
--vscode-symbolIcon-methodForeground: #b180d7;
--vscode-symbolIcon-moduleForeground: #cccccc;
--vscode-symbolIcon-namespaceForeground: #cccccc;
--vscode-symbolIcon-nullForeground: #cccccc;
--vscode-symbolIcon-numberForeground: #cccccc;
--vscode-symbolIcon-objectForeground: #cccccc;
--vscode-symbolIcon-operatorForeground: #cccccc;
--vscode-symbolIcon-packageForeground: #cccccc;
--vscode-symbolIcon-propertyForeground: #cccccc;
--vscode-symbolIcon-referenceForeground: #cccccc;
--vscode-symbolIcon-snippetForeground: #cccccc;
--vscode-symbolIcon-stringForeground: #cccccc;
--vscode-symbolIcon-structForeground: #cccccc;
--vscode-symbolIcon-textForeground: #cccccc;
--vscode-symbolIcon-typeParameterForeground: #cccccc;
--vscode-symbolIcon-unitForeground: #cccccc;
--vscode-symbolIcon-variableForeground: #75beff;
--vscode-editor-lineHighlightBorder: #282828;
--vscode-editor-rangeHighlightBackground: rgba(255, 255, 255, 0.04);
--vscode-editor-symbolHighlightBackground: rgba(234, 92, 0, 0.33);
--vscode-editorCursor-foreground: #aeafad;
--vscode-editorWhitespace-foreground: rgba(227, 228, 226, 0.16);
--vscode-editorIndentGuide-background: #404040;
--vscode-editorIndentGuide-activeBackground: #707070;
--vscode-editorLineNumber-foreground: #858585;
--vscode-editorActiveLineNumber-foreground: #c6c6c6;
--vscode-editorLineNumber-activeForeground: #c6c6c6;
--vscode-editorRuler-foreground: #5a5a5a;
--vscode-editorCodeLens-foreground: #999999;
--vscode-editorBracketMatch-background: rgba(0, 100, 0, 0.1);
--vscode-editorBracketMatch-border: #888888;
--vscode-editorOverviewRuler-border: rgba(127, 127, 127, 0.3);
--vscode-editorGutter-background: #1e1e1e;
--vscode-editorUnnecessaryCode-opacity: rgba(0, 0, 0, 0.67);
--vscode-editorGhostText-foreground: rgba(255, 255, 255, 0.34);
--vscode-editorOverviewRuler-rangeHighlightForeground: rgba(0, 122, 204, 0.6);
--vscode-editorOverviewRuler-errorForeground: rgba(255, 18, 18, 0.7);
--vscode-editorOverviewRuler-warningForeground: #cca700;
--vscode-editorOverviewRuler-infoForeground: #3794ff;
--vscode-editorBracketHighlight-foreground1: #ffd700;
--vscode-editorBracketHighlight-foreground2: #da70d6;
--vscode-editorBracketHighlight-foreground3: #179fff;
--vscode-editorBracketHighlight-foreground4: rgba(0, 0, 0, 0);
--vscode-editorBracketHighlight-foreground5: rgba(0, 0, 0, 0);
--vscode-editorBracketHighlight-foreground6: rgba(0, 0, 0, 0);
--vscode-editorBracketHighlight-unexpectedBracket-foreground: rgba(255, 18, 18, 0.8);
--vscode-editorBracketPairGuide-background1: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-background2: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-background3: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-background4: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-background5: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-background6: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-activeBackground1: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-activeBackground2: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-activeBackground3: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-activeBackground4: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-activeBackground5: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-activeBackground6: rgba(0, 0, 0, 0);
--vscode-editorUnicodeHighlight-border: #bd9b03;
--vscode-editorUnicodeHighlight-background: rgba(189, 155, 3, 0.15);
--vscode-editorOverviewRuler-bracketMatchForeground: #a0a0a0;
--vscode-editor-linkedEditingBackground: rgba(255, 0, 0, 0.3);
--vscode-editor-wordHighlightBackground: rgba(87, 87, 87, 0.72);
--vscode-editor-wordHighlightStrongBackground: rgba(0, 73, 114, 0.72);
--vscode-editor-wordHighlightTextBackground: rgba(87, 87, 87, 0.72);
--vscode-editorOverviewRuler-wordHighlightForeground: rgba(160, 160, 160, 0.8);
--vscode-editorOverviewRuler-wordHighlightStrongForeground: rgba(192, 160, 192, 0.8);
--vscode-editorOverviewRuler-wordHighlightTextForeground: rgba(160, 160, 160, 0.8);
--vscode-peekViewTitle-background: #252526;
--vscode-peekViewTitleLabel-foreground: #ffffff;
--vscode-peekViewTitleDescription-foreground: rgba(204, 204, 204, 0.7);
--vscode-peekView-border: #3794ff;
--vscode-peekViewResult-background: #252526;
--vscode-peekViewResult-lineForeground: #bbbbbb;
--vscode-peekViewResult-fileForeground: #ffffff;
--vscode-peekViewResult-selectionBackground: rgba(51, 153, 255, 0.2);
--vscode-peekViewResult-selectionForeground: #ffffff;
--vscode-peekViewEditor-background: #001f33;
--vscode-peekViewEditorGutter-background: #001f33;
--vscode-peekViewEditorStickyScroll-background: #001f33;
--vscode-peekViewResult-matchHighlightBackground: rgba(234, 92, 0, 0.3);
--vscode-peekViewEditor-matchHighlightBackground: rgba(255, 143, 0, 0.6);
--vscode-editorMarkerNavigationError-background: #f14c4c;
--vscode-editorMarkerNavigationError-headerBackground: rgba(241, 76, 76, 0.1);
--vscode-editorMarkerNavigationWarning-background: #cca700;
--vscode-editorMarkerNavigationWarning-headerBackground: rgba(204, 167, 0, 0.1);
--vscode-editorMarkerNavigationInfo-background: #3794ff;
--vscode-editorMarkerNavigationInfo-headerBackground: rgba(55, 148, 255, 0.1);
--vscode-editorMarkerNavigation-background: #1e1e1e;
--vscode-editorHoverWidget-highlightForeground: #2aaaff;
--vscode-editorSuggestWidget-background: #252526;
--vscode-editorSuggestWidget-border: #454545;
--vscode-editorSuggestWidget-foreground: #d4d4d4;
--vscode-editorSuggestWidget-selectedForeground: #ffffff;
--vscode-editorSuggestWidget-selectedBackground: #04395e;
--vscode-editorSuggestWidget-highlightForeground: #2aaaff;
--vscode-editorSuggestWidget-focusHighlightForeground: #2aaaff;
--vscode-editorSuggestWidgetStatus-foreground: rgba(212, 212, 212, 0.5);
--vscode-editor-foldBackground: rgba(38, 79, 120, 0.3);
--vscode-editorGutter-foldingControlForeground: #c5c5c5; }

.mtk1 { color: #d4d4d4; }
.mtk2 { color: #1e1e1e; }
.mtk3 { color: #cc6666; }
.mtk4 { color: #9cdcfe; }
.mtk5 { color: #ce9178; }
.mtk6 { color: #b5cea8; }
.mtk7 { color: #608b4e; }
.mtk8 { color: #6aa94f; }
.mtk9 { color: #569cd6; }
.mtk10 { color: #f28b82; }
.mtk11 { color: #d7ba7d; }
.mtk12 { color: #dcdcdc; }
.mtk13 { color: #808080; }
.mtk14 { color: #4ec9b0; }
.mtk15 { color: #dcdcaa; }
.mtk16 { color: #f44747; }
.mtk17 { color: #82c6ff; }
.mtk18 { color: #c586c0; }
.mtk19 { color: #a79873; }
.mtk20 { color: #dd6a6f; }
.mtk21 { color: #5bb498; }
.mtk22 { color: #909090; }
.mtk23 { color: #778899; }
.mtk24 { color: #ff00ff; }
.mtk25 { color: #b46695; }
.mtk26 { color: #ff0000; }
.mtk27 { color: #4f76ac; }
.mtk28 { color: #3dc9b0; }
.mtk29 { color: #74b0df; }
.mtk30 { color: #4864aa; }
.mtki { font-style: italic; }
.mtkb { font-weight: bold; }
.mtku { text-decoration: underline; text-underline-position: under; }
.mtks { text-decoration: line-through; }
.mtks.mtku { text-decoration: underline line-through; text-underline-position: under; }</style><script async="async" type="text/javascript" src="./Untitled21.ipynb - Colab_files/markdown.js.download"></script><script async="async" type="text/javascript" src="./Untitled21.ipynb - Colab_files/python.js.download"></script></head><body class="" style="overscroll-behavior: contain;"><div style="visibility: hidden; overflow: hidden; position: absolute; top: 0px; height: 1px; width: auto; padding: 0px; border: 0px; margin: 0px; text-align: left; text-indent: 0px; text-transform: none; line-height: normal; letter-spacing: normal; word-spacing: normal;"><div id="MathJax_Hidden"></div></div><div id="MathJax_Message" style="display: none;"></div><div class="scripts"><script nonce="">window.performance.mark('external_scripts_start');</script><script src="./Untitled21.ipynb - Colab_files/gapi_loader.js.download" nonce=""></script><script src="./Untitled21.ipynb - Colab_files/socketio_binary.js.download" nonce=""></script><script src="./Untitled21.ipynb - Colab_files/analytics_binary.js.download" nonce=""></script><script src="./Untitled21.ipynb - Colab_files/MathJax.js.download" nonce=""></script><script src="./Untitled21.ipynb - Colab_files/js_monaco_editor_vs_loader.js.download" nonce=""></script><script nonce="">window.performance.mark('external_scripts_end'); window.performance.measure('external_scripts', 'external_scripts_start', 'external_scripts_end'); window.performance.mark('colab_load_start');</script><script src="./Untitled21.ipynb - Colab_files/external_binary.js.download" nonce=""></script><script nonce="">
          window.performance.mark('colab_load_end');
          window.performance.measure('colab_load', 'colab_load_start', 'colab_load_end');
        </script></div><colab-snackbar leading="" labeltext="" id="message-area" class="message-area"><template shadowrootmode="open"><!----><style>
        :host .mdc-snackbar__surface {
          background-color: var(--colab-inverse-surface-color);
        }

        :host .mdc-snackbar__label {
          color: var(--colab-inverse-on-surface-color);
        }
      </style>
      <!--?lit$050605479$-->
      <div class="mdc-snackbar mdc-snackbar--leading">
        <div class="mdc-snackbar__surface">
          <!--?lit$050605479$-->
          <div class="mdc-snackbar__actions">
            <slot name="action"></slot>
            <slot name="dismiss"></slot>
          </div>
        </div>
      </div><!--?--></template>
      <md-icon-button class="close" slot="dismiss" title="Close" data-aria-label="Close" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Close">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>close</md-icon>
      </md-icon-button>
    </colab-snackbar><colab-snackbar leading="" labeltext="" id="message-area-secondary" class="message-area startup"><template shadowrootmode="open"><!----><style>
        :host .mdc-snackbar__surface {
          background-color: var(--colab-inverse-surface-color);
        }

        :host .mdc-snackbar__label {
          color: var(--colab-inverse-on-surface-color);
        }
      </style>
      <!--?lit$050605479$-->
      <div class="mdc-snackbar mdc-snackbar--leading">
        <div class="mdc-snackbar__surface">
          <!--?lit$050605479$--><div class="mdc-snackbar__label" role="status" aria-live="polite">Loading...</div>
          <div class="mdc-snackbar__actions">
            <slot name="action"></slot>
            <slot name="dismiss"></slot>
          </div>
        </div>
      </div><!--?--></template>
      <md-icon-button class="close" slot="dismiss" title="Close" data-aria-label="Close" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Close">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>close</md-icon>
      </md-icon-button>
    </colab-snackbar><div ng-non-bindable=""></div><div class="gb_Ac" ng-non-bindable="" style="visibility: hidden; left: 1329px; top: 52px; display: none;"><div class="gb_Bc"><div>Google Account</div><div class="gb_g">Maryam Sayed</div><div>maryamsayed207@gmail.com</div></div></div><script nonce="">this.gbar_=this.gbar_||{};(function(_){var window=this;
try{
var vd;vd=class extends _.gd{};_.wd=function(a,b){if(b in a.i)return a.i[b];throw new vd;};_.xd=function(a){return _.wd(_.dd.i(),a)};
}catch(e){_._DumpException(e)}
try{
/*

 Copyright Google LLC
 SPDX-License-Identifier: Apache-2.0
*/
var Ad;_.yd=function(a){const b=a.length;if(b>0){const c=Array(b);for(let d=0;d<b;d++)c[d]=a[d];return c}return[]};Ad=function(a){return new _.zd(b=>b.substr(0,a.length+1).toLowerCase()===a+":")};_.Bd=globalThis.trustedTypes;_.Cd=class{constructor(a){this.i=a}toString(){return this.i}};_.Dd=new _.Cd("about:invalid#zClosurez");_.zd=class{constructor(a){this.lh=a}};_.Ed=[Ad("data"),Ad("http"),Ad("https"),Ad("mailto"),Ad("ftp"),new _.zd(a=>/^[^:]*([/?#]|$)/.test(a))];_.Fd=class{constructor(a){this.i=a}toString(){return this.i+""}};_.Gd=new _.Fd(_.Bd?_.Bd.emptyHTML:"");
}catch(e){_._DumpException(e)}
try{
var Ld,Zd,Kd,Md,Rd;_.Hd=function(a){return a==null?a:(0,_.Ua)(a)?a|0:void 0};_.Id=function(a){if(a==null)return a;if(typeof a==="string"&&a)a=+a;else if(typeof a!=="number")return;return(0,_.Ua)(a)?a|0:void 0};_.Jd=function(a,b){return a.lastIndexOf(b,0)==0};Ld=function(){let a=null;if(!Kd)return a;try{const b=c=>c;a=Kd.createPolicy("ogb-qtm#html",{createHTML:b,createScript:b,createScriptURL:b})}catch(b){}return a};_.Nd=function(){Md===void 0&&(Md=Ld());return Md};
_.Pd=function(a){const b=_.Nd();return new _.Od(b?b.createScriptURL(a):a)};_.Qd=function(a){if(a instanceof _.Od)return a.i;throw Error("H");};_.Sd=function(a){if(Rd.test(a))return a};_.Td=function(a){if(a instanceof _.Cd)if(a instanceof _.Cd)a=a.i;else throw Error("H");else a=_.Sd(a);return a};_.Ud=function(a,b=document){let c;const d=(c=b.querySelector)==null?void 0:c.call(b,`${a}[nonce]`);return d==null?"":d.nonce||d.getAttribute("nonce")||""};_.Vd=function(a,b,c){return _.tb(a,b,c)!==void 0};
_.Wd=function(a,b){return _.Id(_.Bc(a,b))};_.S=function(a,b){return _.Hd(_.Bc(a,b))};_.T=function(a,b,c=0){let d;return(d=_.Wd(a,b))!=null?d:c};_.Xd=function(a,b,c=0){let d;return(d=_.S(a,b))!=null?d:c};_.Yd=function(a){var b=_.Sa(a);return b=="array"||b=="object"&&typeof a.length=="number"};Kd=_.Bd;_.Od=class{constructor(a){this.i=a}toString(){return this.i+""}};Rd=/^\s*(?!javascript:)(?:[\w+.-]+:|[^:/?#]*(?:[/?#]|$))/i;var de,he,$d;_.be=function(a){return a?new $d(_.ae(a)):Zd||(Zd=new $d)};_.ce=function(a,b){return typeof b==="string"?a.getElementById(b):b};_.U=function(a,b){var c=b||document;c.getElementsByClassName?a=c.getElementsByClassName(a)[0]:(c=document,a?a=(b||c).querySelector(a?"."+a:""):(b=b||c,a=(a?b.querySelectorAll(a?"."+a:""):b.getElementsByTagName("*"))[0]||null));return a||null};
_.ee=function(a,b){_.vb(b,function(c,d){d=="style"?a.style.cssText=c:d=="class"?a.className=c:d=="for"?a.htmlFor=c:de.hasOwnProperty(d)?a.setAttribute(de[d],c):_.Jd(d,"aria-")||_.Jd(d,"data-")?a.setAttribute(d,c):a[d]=c})};de={cellpadding:"cellPadding",cellspacing:"cellSpacing",colspan:"colSpan",frameborder:"frameBorder",height:"height",maxlength:"maxLength",nonce:"nonce",role:"role",rowspan:"rowSpan",type:"type",usemap:"useMap",valign:"vAlign",width:"width"};
_.fe=function(a){return a?a.defaultView:window};_.ie=function(a,b){const c=b[1],d=_.ge(a,String(b[0]));c&&(typeof c==="string"?d.className=c:Array.isArray(c)?d.className=c.join(" "):_.ee(d,c));b.length>2&&he(a,d,b);return d};he=function(a,b,c){function d(e){e&&b.appendChild(typeof e==="string"?a.createTextNode(e):e)}for(let e=2;e<c.length;e++){const f=c[e];!_.Yd(f)||_.Eb(f)&&f.nodeType>0?d(f):_.Xb(f&&typeof f.length=="number"&&typeof f.item=="function"?_.yd(f):f,d)}};
_.je=function(a){return _.ge(document,a)};_.ge=function(a,b){b=String(b);a.contentType==="application/xhtml+xml"&&(b=b.toLowerCase());return a.createElement(b)};_.ke=function(a){let b;for(;b=a.firstChild;)a.removeChild(b)};_.le=function(a){return a&&a.parentNode?a.parentNode.removeChild(a):null};_.me=function(a,b){return a&&b?a==b||a.contains(b):!1};_.ae=function(a){return a.nodeType==9?a:a.ownerDocument||a.document};$d=function(a){this.i=a||_.t.document||document};_.p=$d.prototype;
_.p.H=function(a){return _.ce(this.i,a)};_.p.Ua=function(a,b,c){return _.ie(this.i,arguments)};_.p.appendChild=function(a,b){a.appendChild(b)};_.p.ue=_.ke;_.p.Nf=_.le;_.p.Mf=_.me;
}catch(e){_._DumpException(e)}
try{
_.wi=function(a){const b=_.Ud("script",a.ownerDocument);b&&a.setAttribute("nonce",b)};_.xi=function(a){if(!a)return null;a=_.G(a,4);var b;a===null||a===void 0?b=null:b=_.Pd(a);return b};_.yi=class extends _.P{constructor(a){super(a)}};_.zi=function(a,b){return(b||document).getElementsByTagName(String(a))};
}catch(e){_._DumpException(e)}
try{
var Bi=function(a,b,c){a<b?Ai(a+1,b):_.Oc.log(Error("fa`"+a+"`"+b),{url:c})},Ai=function(a,b){if(Ci){const c=_.je("SCRIPT");c.async=!0;c.type="text/javascript";c.charset="UTF-8";c.src=_.Qd(Ci);_.wi(c);c.onerror=_.Hb(Bi,a,b,c.src);_.zi("HEAD")[0].appendChild(c)}},Di=class extends _.P{constructor(a){super(a)}};var Ei=_.D(_.Yc,Di,17)||new Di,Fi,Ci=(Fi=_.D(Ei,_.yi,1))?_.xi(Fi):null,Gi,Hi=(Gi=_.D(Ei,_.yi,2))?_.xi(Gi):null,Ii=function(){Ai(1,2);if(Hi){const a=_.je("LINK");a.setAttribute("type","text/css");a.href=_.Qd(Hi).toString();a.rel="stylesheet";let b=_.Ud("style",document);b&&a.setAttribute("nonce",b);_.zi("HEAD")[0].appendChild(a)}};(function(){const a=_.Zc();if(_.F(a,18))Ii();else{const b=_.Wd(a,19)||0;window.addEventListener("load",()=>{window.setTimeout(Ii,b)})}})();
}catch(e){_._DumpException(e)}
})(this.gbar_);
// Google Inc.
</script><tldx-lmi-shadow-root data-wxt-shadow-root=""><template shadowrootmode="open">
<!-- saved from url=(0095)https://colab.research.google.com/drive/1SRMnbgb9yKuwM9M4JRgH7FB5Rigi1Y2g#scrollTo=af5FKJF5mMLV -->
<html><head><style>:host{--color-base-100: var(--color-base-100);--color-base-200: var(--color-base-200);--color-base-250: var(--color-base-250);--color-base-300: var(--color-base-300);--color-base-400: var(--color-base-400);--color-base-500: var(--color-base-500);--color-base-600: var(--color-base-600);--color-base-700: var(--color-base-700)}.light,[data-mode=light]{--color-base-100: 255 255 255;--color-base-150: 250 250 255;--color-base-200: 246 245 250;--color-base-250: 237 236 244;--color-base-300: 227 226 237;--color-base-400: 176 174 208;--color-base-500: 90 93 141;--color-base-600: 0 8 82;--color-base-700: 1 1 50}.dark,[data-mode=dark]{--color-base-100: 18 18 18;--color-base-150: 23 23 18;--color-base-200: 34 34 34;--color-base-250: 43 43 43;--color-base-300: 53 53 53;--color-base-400: 116 114 114;--color-base-500: 209 209 209;--color-base-600: 237 237 237;--color-base-700: 255 255 255}*,:before,:after{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }*,:before,:after{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}:before,:after{--tw-content: ""}html,:host{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;-o-tab-size:4;tab-size:4;font-family:ui-sans-serif,system-ui,sans-serif,"Apple Color Emoji","Segoe UI Emoji",Segoe UI Symbol,"Noto Color Emoji";font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,samp,pre{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;letter-spacing:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dl,dd,h1,h2,h3,h4,h5,h6,hr,figure,p,pre{margin:0}fieldset{margin:0;padding:0}legend{padding:0}ol,ul,menu{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{opacity:1;color:#9ca3af}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}button,[role=button]{cursor:pointer}:disabled{cursor:default}img,svg,video,canvas,audio,iframe,embed,object{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]:where(:not([hidden=until-found])){display:none}.tiptap>p.is-empty:before{--tw-text-opacity: 1;color:rgba(var(--color-base-400, 176 174 208) / var(--tw-text-opacity, 1))}.tiptap>p.is-empty:before{content:attr(data-placeholder);float:left;height:0;pointer-events:none}.container{width:100%}@media (min-width: 640px){.container{max-width:640px}}@media (min-width: 768px){.container{max-width:768px}}@media (min-width: 1024px){.container{max-width:1024px}}@media (min-width: 1280px){.container{max-width:1280px}}@media (min-width: 1536px){.container{max-width:1536px}}.pointer-events-none{pointer-events:none}.pointer-events-auto{pointer-events:auto}.visible{visibility:visible}.invisible{visibility:hidden}.collapse{visibility:collapse}.fixed{position:fixed}.\!absolute{position:absolute!important}.absolute{position:absolute}.relative{position:relative}.inset-0{top:0;right:0;bottom:0;left:0}.bottom-2{bottom:.5rem}.bottom-4{bottom:1rem}.bottom-\[2px\]{bottom:2px}.bottom-\[calc\(100\%\+16px\)\]{bottom:calc(100% + 16px)}.left-0{left:0}.left-1\/2{left:50%}.left-2{left:.5rem}.left-4{left:1rem}.left-\[-80px\]{left:-80px}.left-\[50\%\]{left:50%}.right-0{right:0}.right-2{right:.5rem}.right-4{right:1rem}.right-5{right:1.25rem}.right-\[var\(--spacing-large\)\]{right:var(--spacing-large)}.top-1\/2{top:50%}.top-2{top:.5rem}.top-4{top:1rem}.top-\[2px\]{top:2px}.top-\[50\%\]{top:50%}.top-\[calc\(var\(--top-position\)\+var\(--spacing-large\)\)\]{top:calc(var(--top-position) + var(--spacing-large))}.z-10{z-index:10}.z-50{z-index:50}.z-\[10000\]{z-index:10000}.z-\[1000\]{z-index:1000}.z-\[1001\]{z-index:1001}.z-\[100\]{z-index:100}.z-\[110\]{z-index:110}.z-\[1\]{z-index:1}.z-\[30001\]{z-index:30001}.z-\[89\]{z-index:89}.z-\[90\]{z-index:90}.z-\[91\]{z-index:91}.m-0{margin:0}.m-m{margin:1rem}.mx-0{margin-left:0;margin-right:0}.mx-8{margin-left:2rem;margin-right:2rem}.my-2{margin-top:.5rem;margin-bottom:.5rem}.my-4{margin-top:1rem;margin-bottom:1rem}.mb-3{margin-bottom:.75rem}.mb-4{margin-bottom:1rem}.mb-l{margin-bottom:1.5rem}.mb-xs{margin-bottom:.25rem}.ml-1{margin-left:.25rem}.ml-s{margin-left:.5rem}.mt-2{margin-top:.5rem}.mt-4,.mt-m{margin-top:1rem}.mt-s{margin-top:.5rem}.box-border{box-sizing:border-box}.block{display:block}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.grid{display:grid}.contents{display:contents}.\!hidden{display:none!important}.hidden{display:none}.h-0{height:0px}.h-1{height:.25rem}.h-12{height:3rem}.h-4{height:1rem}.h-6{height:1.5rem}.h-7{height:1.75rem}.h-8{height:2rem}.h-9{height:2.25rem}.h-\[16px\]{height:16px}.h-\[17px\]{height:17px}.h-\[184px\]{height:184px}.h-\[1px\]{height:1px}.h-\[25px\]{height:25px}.h-\[28px\]{height:28px}.h-\[2px\]{height:2px}.h-\[32px\]{height:32px}.h-\[36px\]{height:36px}.h-\[37px\]{height:37px}.h-\[54px\]{height:54px}.h-\[60px\]{height:60px}.h-\[62px\]{height:62px}.h-fit{height:-moz-fit-content;height:fit-content}.h-full{height:100%}.h-max{height:-moz-max-content;height:max-content}.max-h-\[320px\]{max-height:320px}.max-h-\[500px\]{max-height:500px}.max-h-full{max-height:100%}.min-h-\[192px\]{min-height:192px}.min-h-\[37px\]{min-height:37px}.min-h-\[40px\]{min-height:40px}.min-h-\[45px\]{min-height:45px}.\!w-\[280px\]{width:280px!important}.\!w-\[calc\(100\%-3px\)\]{width:calc(100% - 3px)!important}.w-0{width:0px}.w-12{width:3rem}.w-3{width:.75rem}.w-4{width:1rem}.w-7{width:1.75rem}.w-9{width:2.25rem}.w-\[200px\]{width:200px}.w-\[220px\]{width:220px}.w-\[222px\]{width:222px}.w-\[350px\]{width:350px}.w-\[390px\]{width:390px}.w-\[45px\]{width:45px}.w-\[514px\]{width:514px}.w-\[60px\]{width:60px}.w-\[70px\]{width:70px}.w-\[9\.33px\]{width:9.33px}.w-\[calc\(100\%-32px\)\]{width:calc(100% - 32px)}.w-\[var\(--chip-input-value-length\)\]{width:var(--chip-input-value-length)}.w-auto{width:auto}.w-fit{width:-moz-fit-content;width:fit-content}.w-full{width:100%}.w-max{width:-moz-max-content;width:max-content}.min-w-0{min-width:0px}.min-w-\[200px\]{min-width:200px}.min-w-\[274px\]{min-width:274px}.min-w-\[280px\]{min-width:280px}.min-w-fit{min-width:-moz-fit-content;min-width:fit-content}.max-w-\[212px\]{max-width:212px}.max-w-\[260px\]{max-width:260px}.max-w-\[340px\]{max-width:340px}.max-w-\[390px\]{max-width:390px}.max-w-\[393px\]{max-width:393px}.max-w-\[600px\]{max-width:600px}.max-w-\[none\]{max-width:none}.max-w-full{max-width:100%}.flex-1{flex:1 1 0%}.flex-shrink-0,.shrink-0{flex-shrink:0}.grow{flex-grow:1}.origin-bottom{transform-origin:bottom}.origin-top{transform-origin:top}.-translate-x-1\/2{--tw-translate-x: -50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.-translate-y-1\/2{--tw-translate-y: -50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-x-\[-140px\]{--tw-translate-x: -140px;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-x-\[-280px\]{--tw-translate-x: -280px;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-x-\[-50\%\]{--tw-translate-x: -50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-y-\[-50\%\]{--tw-translate-y: -50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}@keyframes growFromBottom{0%{opacity:0;transform:scale(.9) translateY(16px)}to{opacity:1;transform:scale(1) translateY(0)}}.animate-grow-from-bottom{animation:growFromBottom .4s cubic-bezier(.28,.84,.42,1)}@keyframes growFromTop{0%{opacity:0;transform:scale(.9) translate(-50%,-16px)}to{opacity:1;transform:scale(1)translate(-50%)}}.animate-grow-from-top{animation:growFromTop .4s cubic-bezier(.28,.84,.42,1)}@keyframes pulse{50%{opacity:.5}}.animate-pulse{animation:pulse 2s cubic-bezier(.4,0,.6,1) infinite}@keyframes spin{to{transform:rotate(360deg)}}.animate-spin{animation:spin 1s linear infinite}.cursor-not-allowed{cursor:not-allowed}.cursor-pointer{cursor:pointer}.touch-none{touch-action:none}.select-none{-webkit-user-select:none;-moz-user-select:none;user-select:none}.select-text{-webkit-user-select:text;-moz-user-select:text;user-select:text}.resize{resize:both}.list-none{list-style-type:none}.appearance-none{-webkit-appearance:none;-moz-appearance:none;appearance:none}.grid-cols-2{grid-template-columns:repeat(2,minmax(0,1fr))}.flex-row{flex-direction:row}.flex-row-reverse{flex-direction:row-reverse}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.place-content-center{place-content:center}.content-start{align-content:flex-start}.items-start{align-items:flex-start}.items-center{align-items:center}.justify-start{justify-content:flex-start}.justify-end{justify-content:flex-end}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.\!gap-s{gap:.5rem!important}.gap-1{gap:.25rem}.gap-2{gap:.5rem}.gap-3{gap:.75rem}.gap-4{gap:1rem}.gap-6{gap:1.5rem}.gap-7{gap:1.75rem}.gap-8{gap:2rem}.gap-\[2px\]{gap:2px}.gap-m{gap:1rem}.gap-s{gap:.5rem}.gap-xs{gap:.25rem}.space-x-3>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0;margin-right:calc(.75rem * var(--tw-space-x-reverse));margin-left:calc(.75rem * calc(1 - var(--tw-space-x-reverse)))}.space-y-1>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 0;margin-top:calc(.25rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(.25rem * var(--tw-space-y-reverse))}.self-start{align-self:flex-start}.self-center{align-self:center}.overflow-hidden{overflow:hidden}.overflow-visible{overflow:visible}.overflow-y-auto{overflow-y:auto}.truncate{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.whitespace-nowrap{white-space:nowrap}.whitespace-pre-wrap{white-space:pre-wrap}.text-wrap{text-wrap:wrap}.break-words{overflow-wrap:break-word}.break-all{word-break:break-all}.rounded{border-radius:.25rem}.rounded-2xl{border-radius:1rem}.rounded-3xl{border-radius:1.5rem}.rounded-\[3px\]{border-radius:3px}.rounded-full{border-radius:9999px}.rounded-lg{border-radius:.5rem}.rounded-md{border-radius:.375rem}.rounded-none{border-radius:0}.border{border-width:1px}.border-0{border-width:0px}.border-\[1px\]{border-width:1px}.border-b-2{border-bottom-width:2px}.border-base-200{--tw-border-opacity: 1;border-color:rgba(var(--color-base-200, 246 245 250) / var(--tw-border-opacity, 1))}.border-base-250{--tw-border-opacity: 1;border-color:rgba(var(--color-base-250, 237 236 244) / var(--tw-border-opacity, 1))}.border-base-300{--tw-border-opacity: 1;border-color:rgba(var(--color-base-300, 227 226 237) / var(--tw-border-opacity, 1))}.border-base-400{--tw-border-opacity: 1;border-color:rgba(var(--color-base-400, 176 174 208) / var(--tw-border-opacity, 1))}.border-base-600{--tw-border-opacity: 1;border-color:rgba(var(--color-base-600, 0 8 82) / var(--tw-border-opacity, 1))}.border-primary-400{--tw-border-opacity: 1;border-color:rgb(29 29 255 / var(--tw-border-opacity, 1))}.border-red-300{--tw-border-opacity: 1;border-color:rgb(237 49 93 / var(--tw-border-opacity, 1))}.border-transparent{border-color:transparent}.bg-\[\#01013166\]{background-color:#01013166}.bg-base-100{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-100, 255 255 255) / var(--tw-bg-opacity, 1))}.bg-base-200{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-200, 246 245 250) / var(--tw-bg-opacity, 1))}.bg-base-250{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-250, 237 236 244) / var(--tw-bg-opacity, 1))}.bg-base-300{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-300, 227 226 237) / var(--tw-bg-opacity, 1))}.bg-base-600{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-600, 0 8 82) / var(--tw-bg-opacity, 1))}.bg-base-700\/50{background-color:rgba(var(--color-base-700, 1 1 50) / .5)}.bg-green-400{--tw-bg-opacity: 1;background-color:rgb(15 163 136 / var(--tw-bg-opacity, 1))}.bg-light-blue-100{--tw-bg-opacity: 1;background-color:rgb(244 250 255 / var(--tw-bg-opacity, 1))}.bg-orange-100{--tw-bg-opacity: 1;background-color:rgb(255 244 240 / var(--tw-bg-opacity, 1))}.bg-primary-100{--tw-bg-opacity: 1;background-color:rgb(242 242 255 / var(--tw-bg-opacity, 1))}.bg-primary-200{--tw-bg-opacity: 1;background-color:rgb(193 193 255 / var(--tw-bg-opacity, 1))}.bg-primary-400{--tw-bg-opacity: 1;background-color:rgb(29 29 255 / var(--tw-bg-opacity, 1))}.bg-primary-500{--tw-bg-opacity: 1;background-color:rgb(0 0 130 / var(--tw-bg-opacity, 1))}.bg-purple-100{--tw-bg-opacity: 1;background-color:rgb(249 241 255 / var(--tw-bg-opacity, 1))}.bg-purple-300{--tw-bg-opacity: 1;background-color:rgb(178 94 244 / var(--tw-bg-opacity, 1))}.bg-red-100{--tw-bg-opacity: 1;background-color:rgb(255 245 247 / var(--tw-bg-opacity, 1))}.bg-red-300{--tw-bg-opacity: 1;background-color:rgb(237 49 93 / var(--tw-bg-opacity, 1))}.bg-slate-500{--tw-bg-opacity: 1;background-color:rgb(100 116 139 / var(--tw-bg-opacity, 1))}.bg-tertiary-100{--tw-bg-opacity: 1;background-color:rgb(249 241 255 / var(--tw-bg-opacity, 1))}.bg-transparent{background-color:transparent}.fill-base-100{fill:rgba(var(--color-base-100, 255 255 255) / 1)}.fill-current{fill:currentColor}.fill-green-400{fill:#0fa388}.stroke-current{stroke:currentColor}.\!p-0{padding:0!important}.p-0{padding:0}.p-1{padding:.25rem}.p-2{padding:.5rem}.p-4{padding:1rem}.p-5{padding:1.25rem}.p-\[2px\]{padding:2px}.p-m{padding:1rem}.p-s{padding:.5rem}.p-xs{padding:.25rem}.\!px-2{padding-left:.5rem!important;padding-right:.5rem!important}.px-1{padding-left:.25rem;padding-right:.25rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-4{padding-left:1rem;padding-right:1rem}.px-6{padding-left:1.5rem;padding-right:1.5rem}.px-8{padding-left:2rem;padding-right:2rem}.px-m{padding-left:1rem;padding-right:1rem}.py-0\.5{padding-top:.125rem;padding-bottom:.125rem}.py-1{padding-top:.25rem;padding-bottom:.25rem}.py-2{padding-top:.5rem;padding-bottom:.5rem}.py-3{padding-top:.75rem;padding-bottom:.75rem}.py-4{padding-top:1rem;padding-bottom:1rem}.py-5{padding-top:1.25rem;padding-bottom:1.25rem}.py-6{padding-top:1.5rem;padding-bottom:1.5rem}.py-\[6px\]{padding-top:6px;padding-bottom:6px}.py-s{padding-top:.5rem;padding-bottom:.5rem}.py-xs{padding-top:.25rem;padding-bottom:.25rem}.\!pr-1{padding-right:.25rem!important}.pb-m{padding-bottom:1rem}.pb-s{padding-bottom:.5rem}.pl-10{padding-left:2.5rem}.pl-2{padding-left:.5rem}.pl-4{padding-left:1rem}.pl-8{padding-left:2rem}.pr-10{padding-right:2.5rem}.pr-8{padding-right:2rem}.pt-2{padding-top:.5rem}.text-left{text-align:left}.text-center{text-align:center}.text-start{text-align:start}.text-2xs{font-size:.625rem}.text-\[10px\]{font-size:10px}.text-\[12px\]{font-size:12px}.text-\[13px\]{font-size:13px}.text-\[14px\]{font-size:14px}.text-\[15px\]{font-size:15px}.text-\[18px\]{font-size:18px}.text-\[21px\]{font-size:21px}.text-\[24px\]{font-size:24px}.text-\[36px\]{font-size:36px}.text-base{font-size:1rem;line-height:1.5rem}.text-lg{font-size:1.125rem;line-height:1.75rem}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xs{font-size:.75rem;line-height:1rem}.font-\[400\]{font-weight:400}.font-\[500\]{font-weight:500}.font-bold{font-weight:700}.font-medium{font-weight:500}.font-normal{font-weight:400}.font-semibold{font-weight:600}.uppercase{text-transform:uppercase}.capitalize{text-transform:capitalize}.italic{font-style:italic}.\!leading-4{line-height:1rem!important}.leading-\[1\.16\]{line-height:1.16}.leading-\[1\.2\]{line-height:1.2}.leading-\[1\.3\]{line-height:1.3}.leading-\[1\.4\]{line-height:1.4}.leading-\[18px\]{line-height:18px}.leading-none{line-height:1}.tracking-\[-1\%\]{letter-spacing:-1%}.tracking-\[-1\.5\%\]{letter-spacing:-1.5%}.tracking-\[-2\%\]{letter-spacing:-2%}.tracking-\[-4\%\]{letter-spacing:-4%}.tracking-normal{letter-spacing:0em}.\!text-base-400{--tw-text-opacity: 1 !important;color:rgba(var(--color-base-400, 176 174 208) / var(--tw-text-opacity, 1))!important}.\!text-base-600{--tw-text-opacity: 1 !important;color:rgba(var(--color-base-600, 0 8 82) / var(--tw-text-opacity, 1))!important}.text-base-100{--tw-text-opacity: 1;color:rgba(var(--color-base-100, 255 255 255) / var(--tw-text-opacity, 1))}.text-base-200{--tw-text-opacity: 1;color:rgba(var(--color-base-200, 246 245 250) / var(--tw-text-opacity, 1))}.text-base-400{--tw-text-opacity: 1;color:rgba(var(--color-base-400, 176 174 208) / var(--tw-text-opacity, 1))}.text-base-500{--tw-text-opacity: 1;color:rgba(var(--color-base-500, 90 93 141) / var(--tw-text-opacity, 1))}.text-base-600{--tw-text-opacity: 1;color:rgba(var(--color-base-600, 0 8 82) / var(--tw-text-opacity, 1))}.text-base-700{--tw-text-opacity: 1;color:rgba(var(--color-base-700, 1 1 50) / var(--tw-text-opacity, 1))}.text-blue-400{--tw-text-opacity: 1;color:rgb(96 165 250 / var(--tw-text-opacity, 1))}.text-gray-600{--tw-text-opacity: 1;color:rgb(75 85 99 / var(--tw-text-opacity, 1))}.text-green-400{--tw-text-opacity: 1;color:rgb(15 163 136 / var(--tw-text-opacity, 1))}.text-light-blue-400{--tw-text-opacity: 1;color:rgb(0 141 255 / var(--tw-text-opacity, 1))}.text-orange-400{--tw-text-opacity: 1;color:rgb(255 107 70 / var(--tw-text-opacity, 1))}.text-primary-300{--tw-text-opacity: 1;color:rgb(133 133 255 / var(--tw-text-opacity, 1))}.text-primary-400{--tw-text-opacity: 1;color:rgb(29 29 255 / var(--tw-text-opacity, 1))}.text-purple-300{--tw-text-opacity: 1;color:rgb(178 94 244 / var(--tw-text-opacity, 1))}.text-red-300{--tw-text-opacity: 1;color:rgb(237 49 93 / var(--tw-text-opacity, 1))}.text-red-400{--tw-text-opacity: 1;color:rgb(181 3 44 / var(--tw-text-opacity, 1))}.text-tertiary-300{--tw-text-opacity: 1;color:rgb(178 94 244 / var(--tw-text-opacity, 1))}.text-white{--tw-text-opacity: 1;color:rgb(255 255 255 / var(--tw-text-opacity, 1))}.underline{text-decoration-line:underline}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.opacity-0{opacity:0}.opacity-30{opacity:.3}.opacity-40{opacity:.4}.opacity-65{opacity:.65}.shadow{--tw-shadow: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--tw-shadow-colored: 0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.shadow-lg{--tw-shadow: 0px 5px 30px 0px rgba(var(--color-base-600) / .1);--tw-shadow-colored: 0px 5px 30px 0px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.shadow-md{--tw-shadow: 0px 5px 20px 0px rgba(var(--color-base-600) / .05);--tw-shadow-colored: 0px 5px 20px 0px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.shadow-sm{--tw-shadow: 0px 2px 20px 0px rgba(var(--color-base-600) / .03);--tw-shadow-colored: 0px 2px 20px 0px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.outline-none{outline:2px solid transparent;outline-offset:2px}.outline{outline-style:solid}.outline-\[4\.5px\]{outline-width:4.5px}.outline-tertiary-400{outline-color:#953bab}.ring-base-200{--tw-ring-opacity: 1;--tw-ring-color: rgba(var(--color-base-200, 246 245 250) / var(--tw-ring-opacity, 1))}.ring-primary-400\/10{--tw-ring-color: rgb(29 29 255 / .1)}.ring-purple-300\/10{--tw-ring-color: rgb(178 94 244 / .1)}.ring-red-300\/10{--tw-ring-color: rgb(237 49 93 / .1)}.blur{--tw-blur: blur(8px);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.transition{transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.transition-\[background-color\]{transition-property:background-color;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.transition-all{transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.transition-colors{transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.duration-200{transition-duration:.2s}.ease-in-out{transition-timing-function:cubic-bezier(.4,0,.2,1)}.ease-linear{transition-timing-function:linear}@keyframes enter{0%{opacity:var(--tw-enter-opacity, 1);transform:translate3d(var(--tw-enter-translate-x, 0),var(--tw-enter-translate-y, 0),0) scale3d(var(--tw-enter-scale, 1),var(--tw-enter-scale, 1),var(--tw-enter-scale, 1)) rotate(var(--tw-enter-rotate, 0))}}@keyframes exit{to{opacity:var(--tw-exit-opacity, 1);transform:translate3d(var(--tw-exit-translate-x, 0),var(--tw-exit-translate-y, 0),0) scale3d(var(--tw-exit-scale, 1),var(--tw-exit-scale, 1),var(--tw-exit-scale, 1)) rotate(var(--tw-exit-rotate, 0))}}.duration-200{animation-duration:.2s}.ease-in-out{animation-timing-function:cubic-bezier(.4,0,.2,1)}.ease-linear{animation-timing-function:linear}.running{animation-play-state:running}.paused{animation-play-state:paused}.placeholder\:text-sm::-moz-placeholder{font-size:.875rem;line-height:1.25rem}.placeholder\:text-sm::placeholder{font-size:.875rem;line-height:1.25rem}.placeholder\:font-normal::-moz-placeholder{font-weight:400}.placeholder\:font-normal::placeholder{font-weight:400}.placeholder\:text-base-400::-moz-placeholder{--tw-text-opacity: 1;color:rgba(var(--color-base-400, 176 174 208) / var(--tw-text-opacity, 1))}.placeholder\:text-base-400::placeholder{--tw-text-opacity: 1;color:rgba(var(--color-base-400, 176 174 208) / var(--tw-text-opacity, 1))}.before\:absolute:before{content:var(--tw-content);position:absolute}.before\:bottom-0:before{content:var(--tw-content);bottom:0}.before\:left-0:before{content:var(--tw-content);left:0}.before\:top-0:before{content:var(--tw-content);top:0}.before\:flex:before{content:var(--tw-content);display:flex}.before\:h-4:before{content:var(--tw-content);height:1rem}.before\:w-4:before{content:var(--tw-content);width:1rem}.before\:w-\[var\(--player-buffer-progress\)\]:before{content:var(--tw-content);width:var(--player-buffer-progress)}.before\:content-normal:before{content:var(--tw-content);align-content:normal}.before\:rounded-full:before{content:var(--tw-content);border-radius:9999px}.before\:bg-base-400:before{content:var(--tw-content);--tw-bg-opacity: 1;background-color:rgba(var(--color-base-400, 176 174 208) / var(--tw-bg-opacity, 1))}.before\:bg-primary-300:before{content:var(--tw-content);--tw-bg-opacity: 1;background-color:rgb(133 133 255 / var(--tw-bg-opacity, 1))}.before\:transition-\[border\]:before{content:var(--tw-content);transition-property:border;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.before\:transition-\[width\]:before{content:var(--tw-content);transition-property:width;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.before\:content-\[\'\'\]:before{--tw-content: "";content:var(--tw-content)}.after\:absolute:after{content:var(--tw-content);position:absolute}.after\:bottom-0:after{content:var(--tw-content);bottom:0}.after\:left-0:after{content:var(--tw-content);left:0}.after\:top-0:after{content:var(--tw-content);top:0}.after\:flex:after{content:var(--tw-content);display:flex}.after\:w-\[var\(--player-timeline-progress\)\]:after{content:var(--tw-content);width:var(--player-timeline-progress)}.after\:content-normal:after{content:var(--tw-content);align-content:normal}.after\:bg-primary-400:after{content:var(--tw-content);--tw-bg-opacity: 1;background-color:rgb(29 29 255 / var(--tw-bg-opacity, 1))}.after\:transition-\[width\]:after{content:var(--tw-content);transition-property:width;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.checked\:border-\[5px\]:checked{border-width:5px}.checked\:border-none:checked{border-style:none}.checked\:border-primary-400:checked{--tw-border-opacity: 1;border-color:rgb(29 29 255 / var(--tw-border-opacity, 1))}.checked\:bg-primary-400:checked{--tw-bg-opacity: 1;background-color:rgb(29 29 255 / var(--tw-bg-opacity, 1))}.before\:checked\:border-\[5px\]:checked:before{content:var(--tw-content);border-width:5px}.before\:checked\:border-primary-400:checked:before{content:var(--tw-content);--tw-border-opacity: 1;border-color:rgb(29 29 255 / var(--tw-border-opacity, 1))}.hover\:rounded-lg:hover{border-radius:.5rem}.hover\:bg-base-200:hover{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-200, 246 245 250) / var(--tw-bg-opacity, 1))}.hover\:bg-base-250:hover{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-250, 237 236 244) / var(--tw-bg-opacity, 1))}.hover\:bg-primary-500:hover{--tw-bg-opacity: 1;background-color:rgb(0 0 130 / var(--tw-bg-opacity, 1))}.hover\:bg-purple-400:hover{--tw-bg-opacity: 1;background-color:rgb(149 59 171 / var(--tw-bg-opacity, 1))}.hover\:bg-red-400:hover{--tw-bg-opacity: 1;background-color:rgb(181 3 44 / var(--tw-bg-opacity, 1))}.hover\:bg-transparent:hover{background-color:transparent}.hover\:bg-none:hover{background-image:none}.hover\:text-primary-500:hover{--tw-text-opacity: 1;color:rgb(0 0 130 / var(--tw-text-opacity, 1))}.focus\:border-primary-300:focus{--tw-border-opacity: 1;border-color:rgb(133 133 255 / var(--tw-border-opacity, 1))}.focus\:border-red-300:focus{--tw-border-opacity: 1;border-color:rgb(237 49 93 / var(--tw-border-opacity, 1))}.focus\:bg-base-100:focus{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-100, 255 255 255) / var(--tw-bg-opacity, 1))}.focus\:bg-base-200:focus{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-200, 246 245 250) / var(--tw-bg-opacity, 1))}.focus\:bg-transparent:focus{background-color:transparent}.focus\:bg-none:focus{background-image:none}.focus\:text-base-600:focus{--tw-text-opacity: 1;color:rgba(var(--color-base-600, 0 8 82) / var(--tw-text-opacity, 1))}.focus\:outline-none:focus{outline:2px solid transparent;outline-offset:2px}.focus\:placeholder\:text-base-400:focus::-moz-placeholder{--tw-text-opacity: 1;color:rgba(var(--color-base-400, 176 174 208) / var(--tw-text-opacity, 1))}.focus\:placeholder\:text-base-400:focus::placeholder{--tw-text-opacity: 1;color:rgba(var(--color-base-400, 176 174 208) / var(--tw-text-opacity, 1))}.focus-visible\:ring:focus-visible{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(3px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)}.active\:bg-base-200:active{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-200, 246 245 250) / var(--tw-bg-opacity, 1))}.active\:bg-primary-500:active{--tw-bg-opacity: 1;background-color:rgb(0 0 130 / var(--tw-bg-opacity, 1))}.active\:bg-purple-400:active{--tw-bg-opacity: 1;background-color:rgb(149 59 171 / var(--tw-bg-opacity, 1))}.active\:bg-red-400:active{--tw-bg-opacity: 1;background-color:rgb(181 3 44 / var(--tw-bg-opacity, 1))}.disabled\:pointer-events-none:disabled{pointer-events:none}.disabled\:\!cursor-not-allowed:disabled{cursor:not-allowed!important}.disabled\:cursor-not-allowed:disabled{cursor:not-allowed}.disabled\:border-base-300:disabled{--tw-border-opacity: 1;border-color:rgba(var(--color-base-300, 227 226 237) / var(--tw-border-opacity, 1))}.disabled\:bg-base-150:disabled{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-150, 250 250 255) / var(--tw-bg-opacity, 1))}.disabled\:bg-base-200:disabled{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-200, 246 245 250) / var(--tw-bg-opacity, 1))}.disabled\:bg-base-300:disabled{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-300, 227 226 237) / var(--tw-bg-opacity, 1))}.disabled\:text-base-400:disabled{--tw-text-opacity: 1;color:rgba(var(--color-base-400, 176 174 208) / var(--tw-text-opacity, 1))}.disabled\:\!opacity-50:disabled{opacity:.5!important}.disabled\:opacity-30:disabled{opacity:.3}.disabled\:opacity-50:disabled{opacity:.5}.disabled\:before\:checked\:border-base-300:checked:disabled:before{content:var(--tw-content);--tw-border-opacity: 1;border-color:rgba(var(--color-base-300, 227 226 237) / var(--tw-border-opacity, 1))}.disabled\:hover\:\!bg-transparent:hover:disabled{background-color:transparent!important}.disabled\:hover\:bg-transparent:hover:disabled{background-color:transparent}.group\/highlight:hover .group-hover\/highlight\:\!flex{display:flex!important}.group\/trigger:hover .group-hover\/trigger\:flex{display:flex}.has-\[\:focus\]\:border-primary-300:has(:focus){--tw-border-opacity: 1;border-color:rgb(133 133 255 / var(--tw-border-opacity, 1))}.has-\[\:focus\]\:bg-base-100:has(:focus){--tw-bg-opacity: 1;background-color:rgba(var(--color-base-100, 255 255 255) / var(--tw-bg-opacity, 1))}.has-\[\:focus\]\:bg-base-200:has(:focus){--tw-bg-opacity: 1;background-color:rgba(var(--color-base-200, 246 245 250) / var(--tw-bg-opacity, 1))}.has-\[svg\:first-child\]\:pl-2:has(svg:first-child){padding-left:.5rem}.has-\[svg\:first-child\]\:pl-3:has(svg:first-child){padding-left:.75rem}.has-\[svg\:first-child\]\:pl-4:has(svg:first-child){padding-left:1rem}.has-\[svg\:first-child\]\:pl-5:has(svg:first-child){padding-left:1.25rem}.has-\[svg\:first-child\]\:pr-4:has(svg:first-child){padding-right:1rem}.has-\[svg\:first-child\]\:pr-8:has(svg:first-child){padding-right:2rem}.has-\[svg\:last-child\]\:pl-4:has(svg:last-child){padding-left:1rem}.has-\[svg\:last-child\]\:pl-8:has(svg:last-child){padding-left:2rem}.has-\[svg\:last-child\]\:pr-2:has(svg:last-child){padding-right:.5rem}.has-\[svg\:last-child\]\:pr-3:has(svg:last-child){padding-right:.75rem}.has-\[svg\:last-child\]\:pr-4:has(svg:last-child){padding-right:1rem}.has-\[svg\:last-child\]\:pr-5:has(svg:last-child){padding-right:1.25rem}.aria-\[current\=page\]\:border-b-primary-400[aria-current=page]{--tw-border-opacity: 1;border-bottom-color:rgb(29 29 255 / var(--tw-border-opacity, 1))}.aria-\[current\=page\]\:bg-primary-400\/10[aria-current=page]{background-color:#1d1dff1a}.aria-\[current\=page\]\:text-primary-400[aria-current=page]{--tw-text-opacity: 1;color:rgb(29 29 255 / var(--tw-text-opacity, 1))}.aria-\[current\=page\]\:hover\:border-b-primary-500:hover[aria-current=page]{--tw-border-opacity: 1;border-bottom-color:rgb(0 0 130 / var(--tw-border-opacity, 1))}.aria-\[current\=page\]\:hover\:bg-primary-400\/20:hover[aria-current=page]{background-color:#1d1dff33}.aria-\[current\=page\]\:hover\:text-primary-500:hover[aria-current=page]{--tw-text-opacity: 1;color:rgb(0 0 130 / var(--tw-text-opacity, 1))}.group\/dropdown-subtrigger[aria-expanded=true] .group-aria-\[expanded\=true\]\/dropdown-subtrigger\:bg-base-200{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-200, 246 245 250) / var(--tw-bg-opacity, 1))}.data-\[clickable\=false\]\:pointer-events-none[data-clickable=false],.data-\[disabled\=true\]\:pointer-events-none[data-disabled=true],.data-\[loading\=true\]\:pointer-events-none[data-loading=true]{pointer-events:none}.data-\[disabled\=false\]\:pointer-events-auto[data-disabled=false]{pointer-events:auto}.data-\[size\=l\]\:left-\[17px\][data-size=l]{left:17px}.data-\[size\=l\]\:top-\[14px\][data-size=l]{top:14px}.data-\[size\=m\]\:left-\[12px\][data-size=m]{left:12px}.data-\[size\=m\]\:top-\[9px\][data-size=m]{top:9px}.data-\[size\=s\]\:left-\[8px\][data-size=s]{left:8px}.data-\[size\=s\]\:top-\[6px\][data-size=s]{top:6px}.data-\[size\=xl\]\:left-\[23px\][data-size=xl]{left:23px}.data-\[size\=xl\]\:top-\[18px\][data-size=xl]{top:18px}.data-\[size\=xs\]\:left-\[7px\][data-size=xs]{left:7px}.data-\[size\=xs\]\:top-\[10px\][data-size=xs]{top:10px}.data-\[size\=\"big\"\]\:h-\[37px\][data-size=big]{height:37px}.data-\[size\=\"small\"\]\:h-6[data-size=small]{height:1.5rem}.data-\[size\=l\]\:h-8[data-size=l]{height:2rem}.data-\[size\=m\]\:h-6[data-size=m]{height:1.5rem}.data-\[size\=s\]\:h-4[data-size=s]{height:1rem}.data-\[size\=xl\]\:h-10[data-size=xl]{height:2.5rem}.data-\[size\=xs\]\:h-3[data-size=xs]{height:.75rem}.data-\[ai-onboarding\=true\]\:min-h-\[299px\][data-ai-onboarding=true]{min-height:299px}.data-\[path\=auto-share\]\:min-h-\[275px\][data-path=auto-share]{min-height:275px}.data-\[size\=l\]\:w-8[data-size=l]{width:2rem}.data-\[size\=m\]\:w-6[data-size=m]{width:1.5rem}.data-\[size\=s\]\:w-4[data-size=s]{width:1rem}.data-\[size\=xl\]\:w-10[data-size=xl]{width:2.5rem}.data-\[size\=xs\]\:w-3[data-size=xs]{width:.75rem}.data-\[clickable\=true\]\:cursor-pointer[data-clickable=true]{cursor:pointer}.data-\[disabled\=\"true\"\]\:cursor-not-allowed[data-disabled=true]{cursor:not-allowed}.data-\[disabled\=true\]\:\!cursor-not-allowed[data-disabled=true]{cursor:not-allowed!important}.data-\[disabled\=true\]\:cursor-not-allowed[data-disabled=true],.data-\[disabled\]\:cursor-not-allowed[data-disabled],.data-\[loading\=true\]\:cursor-not-allowed[data-loading=true]{cursor:not-allowed}.data-\[outline\=\"true\"\]\:border-\[1px\][data-outline=true]{border-width:1px}.data-\[focus\=true\]\:border-primary-300[data-focus=true]{--tw-border-opacity: 1;border-color:rgb(133 133 255 / var(--tw-border-opacity, 1))}.data-\[variant\=\"primary\"\]\:border-primary-400[data-variant=primary]{--tw-border-opacity: 1;border-color:rgb(29 29 255 / var(--tw-border-opacity, 1))}.data-\[variant\=\"secondary\"\]\:border-base-400[data-variant=secondary]{--tw-border-opacity: 1;border-color:rgba(var(--color-base-400, 176 174 208) / var(--tw-border-opacity, 1))}.data-\[checked\=false\]\:bg-base-200[data-checked=false]{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-200, 246 245 250) / var(--tw-bg-opacity, 1))}.data-\[checked\=true\]\:bg-green-100[data-checked=true]{--tw-bg-opacity: 1;background-color:rgb(235 255 251 / var(--tw-bg-opacity, 1))}.data-\[disabled\]\:bg-base-150[data-disabled]{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-150, 250 250 255) / var(--tw-bg-opacity, 1))}.data-\[disabled\]\:bg-base-200[data-disabled],.data-\[selected\=true\]\:bg-base-200[data-selected=true]{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-200, 246 245 250) / var(--tw-bg-opacity, 1))}.data-\[variant\=\"primary\"\]\:bg-primary-100[data-variant=primary]{--tw-bg-opacity: 1;background-color:rgb(242 242 255 / var(--tw-bg-opacity, 1))}.data-\[variant\=\"secondary\"\]\:bg-base-200[data-variant=secondary]{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-200, 246 245 250) / var(--tw-bg-opacity, 1))}.data-\[variant\=\"tertiary\"\]\:bg-tertiary-100[data-variant=tertiary]{--tw-bg-opacity: 1;background-color:rgb(249 241 255 / var(--tw-bg-opacity, 1))}.data-\[size\=m\]\:p-4[data-size=m]{padding:1rem}.data-\[size\=s\]\:p-2[data-size=s]{padding:.5rem}.data-\[size\=\"big\"\]\:py-2[data-size=big]{padding-top:.5rem;padding-bottom:.5rem}.data-\[size\=\"small\"\]\:py-\[6px\][data-size=small]{padding-top:6px;padding-bottom:6px}.data-\[has-cta\=false\]\:text-center[data-has-cta=false]{text-align:center}.data-\[size\=m\]\:text-\[15px\][data-size=m]{font-size:15px}.data-\[size\=s\]\:text-xs[data-size=s]{font-size:.75rem;line-height:1rem}.data-\[disabled\=false\]\:\!opacity-100[data-disabled=false]{opacity:1!important}.data-\[disabled\=true\]\:\!opacity-50[data-disabled=true]{opacity:.5!important}.data-\[disabled\=true\]\:opacity-50[data-disabled=true]{opacity:.5}.data-\[disabled\]\:opacity-30[data-disabled],.data-\[loading\=true\]\:opacity-30[data-loading=true]{opacity:.3}.data-\[outline\=true\]\:outline[data-outline=true]{outline-style:solid}.data-\[outline\=true\]\:outline-\[1\.5px\][data-outline=true]{outline-width:1.5px}.data-\[outline\=true\]\:outline-primary-400[data-outline=true]{outline-color:#1d1dff}.data-\[attached\=true\]\:first\:rounded-r-none:first-child[data-attached=true]{border-top-right-radius:0;border-bottom-right-radius:0}.data-\[attached\=true\]\:first\:border-r-0:first-child[data-attached=true]{border-right-width:0px}.data-\[attached\=true\]\:last\:rounded-l-none:last-child[data-attached=true]{border-top-left-radius:0;border-bottom-left-radius:0}.data-\[attached\=true\]\:last\:border-l-0:last-child[data-attached=true]{border-left-width:0px}.data-\[disabled\=true\]\:hover\:\!bg-transparent:hover[data-disabled=true]{background-color:transparent!important}.data-\[variant\=\"secondary\"\]\:hover\:bg-base-250:hover[data-variant=secondary]{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-250, 237 236 244) / var(--tw-bg-opacity, 1))}.group\/dropdown-wordtrigger[data-state=closed] .group-data-\[state\=closed\]\/dropdown-wordtrigger\:block,.group\/dropdown-wordtrigger[data-state=open] .group-data-\[state\=open\]\/dropdown-wordtrigger\:block{display:block}.group\/trigger[data-state=paused] .group-data-\[state\=paused\]\/trigger\:flex,.group\/trigger[data-state=playing] .group-data-\[state\=playing\]\/trigger\:flex{display:flex}.group\/checkbox[data-checked=false] .group-data-\[checked\=false\]\/checkbox\:hidden,.group\/sidebar[data-state=collapsed] .group-data-\[state\=\"collapsed\"\]\/sidebar\:hidden,.group\/sidebar[data-state=expanded] .group-data-\[state\=\"expanded\"\]\/sidebar\:hidden,.group\/combobox-trigger[data-state=closed] .group-data-\[state\=closed\]\/combobox-trigger\:hidden,.group\/dropdown-wordtrigger[data-state=closed] .group-data-\[state\=closed\]\/dropdown-wordtrigger\:hidden,.group\/combobox-trigger[data-state=open] .group-data-\[state\=open\]\/combobox-trigger\:hidden,.group\/dropdown-wordtrigger[data-state=open] .group-data-\[state\=open\]\/dropdown-wordtrigger\:hidden{display:none}.group\/button[data-size=lg] .group-data-\[size\=\"lg\"\]\/button\:h-6{height:1.5rem}.group\/button[data-size=md] .group-data-\[size\=\"md\"\]\/button\:h-5{height:1.25rem}.group\/button[data-size=sm] .group-data-\[size\=\"sm\"\]\/button\:h-4{height:1rem}.group\/button[data-size=xl] .group-data-\[size\=\"xl\"\]\/button\:h-7{height:1.75rem}.group\/button[data-size=lg] .group-data-\[size\=\"lg\"\]\/button\:w-6{width:1.5rem}.group\/button[data-size=md] .group-data-\[size\=\"md\"\]\/button\:w-5{width:1.25rem}.group\/button[data-size=sm] .group-data-\[size\=\"sm\"\]\/button\:w-4{width:1rem}.group\/button[data-size=xl] .group-data-\[size\=\"xl\"\]\/button\:w-7{width:1.75rem}.group\/dropdown-item[data-size=m] .group-data-\[size\=m\]\/dropdown-item\:\!w-5{width:1.25rem!important}.group\/dropdown-item[data-size=s] .group-data-\[size\=s\]\/dropdown-item\:w-m{width:1rem}.group\/sidebar[data-state=collapsed] .group-data-\[state\=\"collapsed\"\]\/sidebar\:justify-center{justify-content:center}.group\/input-root[data-invalid=true] .group-data-\[invalid\=true\]\/input-root\:border-red-300{--tw-border-opacity: 1;border-color:rgb(237 49 93 / var(--tw-border-opacity, 1))}.group\/sidebar[data-type=light] .group-data-\[type\=\"light\"\]\/sidebar\:bg-base-100{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-100, 255 255 255) / var(--tw-bg-opacity, 1))}.group\/tooltip[data-type=default] .group-data-\[type\=\"default\"\]\/tooltip\:fill-base-600{fill:rgba(var(--color-base-600, 0 8 82) / 1)}.group\/tooltip[data-type=error] .group-data-\[type\=\"error\"\]\/tooltip\:fill-red-300{fill:#ed315d}.group\/tooltip[data-type=success] .group-data-\[type\=\"success\"\]\/tooltip\:fill-green-400{fill:#0fa388}.group\/sidebar[data-state=collapsed] .group-data-\[state\=\"collapsed\"\]\/sidebar\:px-1{padding-left:.25rem;padding-right:.25rem}.group\/chip[data-size=big] .group-data-\[size\=\"big\"\]\/chip\:text-s{font-size:.938rem}.group\/chip[data-size=small] .group-data-\[size\=\"small\"\]\/chip\:text-2xs{font-size:.625rem}.group\/dropdown-item[data-size=m] .group-data-\[size\=m\]\/dropdown-item\:\!text-\[15px\]{font-size:15px!important}.group\/dropdown-item[data-size=s] .group-data-\[size\=s\]\/dropdown-item\:text-xs{font-size:.75rem;line-height:1rem}.group\/combobox-root[data-invalid=true] .group-data-\[invalid\=true\]\/combobox-root\:text-red-300,.group\/input-root[data-invalid=true] .group-data-\[invalid\=true\]\/input-root\:text-red-300{--tw-text-opacity: 1;color:rgb(237 49 93 / var(--tw-text-opacity, 1))}.group\/banner[data-type=secondary] .group-data-\[type\=\"secondary\"\]\/banner\:text-base-100{--tw-text-opacity: 1;color:rgba(var(--color-base-100, 255 255 255) / var(--tw-text-opacity, 1))}.group\/chip[data-variant=primary] .group-data-\[variant\=\"primary\"\]\/chip\:text-primary-400{--tw-text-opacity: 1;color:rgb(29 29 255 / var(--tw-text-opacity, 1))}.group\/chip[data-variant=secondary] .group-data-\[variant\=\"secondary\"\]\/chip\:text-base-400{--tw-text-opacity: 1;color:rgba(var(--color-base-400, 176 174 208) / var(--tw-text-opacity, 1))}.group\/chip[data-variant=tertiary] .group-data-\[variant\=\"tertiary\"\]\/chip\:text-base-300{--tw-text-opacity: 1;color:rgba(var(--color-base-300, 227 226 237) / var(--tw-text-opacity, 1))}.group\/chip[data-variant=tertiary] .group-data-\[variant\=\"tertiary\"\]\/chip\:text-tertiary-300{--tw-text-opacity: 1;color:rgb(178 94 244 / var(--tw-text-opacity, 1))}.group\/sidebar[data-type=light] .group-data-\[type\=\"light\"\]\/sidebar\:hover\:bg-base-150:hover{--tw-bg-opacity: 1;background-color:rgba(var(--color-base-150, 250 250 255) / var(--tw-bg-opacity, 1))}.group\/input-root[data-invalid=true] .group-data-\[invalid\=true\]\/input-root\:focus\:border-red-300:focus{--tw-border-opacity: 1;border-color:rgb(237 49 93 / var(--tw-border-opacity, 1))}.group\/chip:hover[data-variant=primary] .group-hover\/chip\:group-data-\[variant\=\"primary\"\]\/chip\:text-primary-500{--tw-text-opacity: 1;color:rgb(0 0 130 / var(--tw-text-opacity, 1))}.group\/chip:hover[data-variant=secondary] .group-hover\/chip\:group-data-\[variant\=\"secondary\"\]\/chip\:text-base-500{--tw-text-opacity: 1;color:rgba(var(--color-base-500, 90 93 141) / var(--tw-text-opacity, 1))}.group\/chip:hover[data-variant=tertiary] .group-hover\/chip\:group-data-\[variant\=\"tertiary\"\]\/chip\:text-tertiary-400{--tw-text-opacity: 1;color:rgb(149 59 171 / var(--tw-text-opacity, 1))}.group\/sidebar[data-type=light] .group-data-\[type\=\"light\"\]\/sidebar\:aria-\[current\=page\]\:bg-primary-400\/10[aria-current=page]{background-color:#1d1dff1a}.group\/sidebar[data-type=light] .group-data-\[type\=\"light\"\]\/sidebar\:aria-\[current\=page\]\:hover\:bg-primary-400\/20:hover[aria-current=page]{background-color:#1d1dff33}@media not all and (min-width: 1024px){.group\/sidebar:hover .max-lg\:group-hover\/sidebar\:\!px-4{padding-left:1rem!important;padding-right:1rem!important}.group\/sidebar[data-state=default] .max-lg\:group-data-\[state\=\"default\"\]\/sidebar\:hidden{display:none}}@media not all and (min-width: 768px){.group\/sidebar:hover .group-hover\/sidebar\:max-md\:\!px-4{padding-left:1rem!important;padding-right:1rem!important}.group\/sidebar[data-state=default] .max-md\:group-data-\[state\=\"default\"\]\/sidebar\:justify-center{justify-content:center}.group\/sidebar[data-state=default] .max-md\:group-data-\[state\=\"default\"\]\/sidebar\:px-1{padding-left:.25rem;padding-right:.25rem}}@media (min-width: 768px){.md\:text-\[15px\]{font-size:15px}.md\:text-\[16px\]{font-size:16px}.md\:text-\[21px\]{font-size:21px}.md\:text-\[24px\]{font-size:24px}.md\:text-\[28px\]{font-size:28px}.md\:text-\[36px\]{font-size:36px}.md\:text-\[52px\]{font-size:52px}.md\:leading-\[1\.16\]{line-height:1.16}.md\:leading-\[1\.25\]{line-height:1.25}.md\:leading-\[1\.2\]{line-height:1.2}.md\:leading-\[1\.4\]{line-height:1.4}.md\:tracking-\[-1\%\]{letter-spacing:-1%}.md\:tracking-\[-2\%\]{letter-spacing:-2%}.md\:tracking-\[-3\%\]{letter-spacing:-3%}.group\/sidebar[data-state=default] .md\:group-data-\[state\=\"default\"\]\/sidebar\:hidden{display:none}}.\[\&\>\*\]\:outline-none>*{outline:2px solid transparent;outline-offset:2px}.group\/banner[data-type=secondary] .group-data-\[type\=\"secondary\"\]\/banner\:\[\&\>\*\]\:\!text-base-100>*{--tw-text-opacity: 1 !important;color:rgba(var(--color-base-100, 255 255 255) / var(--tw-text-opacity, 1))!important}.data-\[attached\=true\]\:\[\&\>not\(\:first-child\,_\:last-child\)\]\:rounded-none>not(:first-child,:last-child)[data-attached="true"]{border-radius:0}.\[\&\>span\]\:\!no-underline>span{text-decoration-line:none!important}.\[\&\>svg\]\:gap-xs>svg{gap:.25rem}.\[\&_\>_div_\>_p\]\:data-\[disabled\]\:text-base-400[data-disabled]>div>p{--tw-text-opacity: 1;color:rgba(var(--color-base-400, 176 174 208) / var(--tw-text-opacity, 1))}.\[\&_button\>span\]\:text-base-500 button>span{--tw-text-opacity: 1;color:rgba(var(--color-base-500, 90 93 141) / var(--tw-text-opacity, 1))}.\[\&_button\>span\]\:text-orange-400 button>span{--tw-text-opacity: 1;color:rgb(255 107 70 / var(--tw-text-opacity, 1))}.\[\&_button\>span\]\:text-white button>span{--tw-text-opacity: 1;color:rgb(255 255 255 / var(--tw-text-opacity, 1))}.\[\&_button\>svg\]\:fill-light-blue-400 button>svg{fill:#008dff}.\[\&_button\>svg\]\:fill-orange-400 button>svg{fill:#ff6b46}.\[\&_button\>svg\]\:fill-primary-400 button>svg{fill:#1d1dff}.\[\&_button\>svg\]\:fill-purple-300 button>svg{fill:#b25ef4}.\[\&_button\>svg\]\:fill-white button>svg{fill:#fff}*{font-family:Work Sans,sans-serif}</style></head><body><div></div></body></html></template></tldx-lmi-shadow-root><div id="tldx-toast-container"></div><div style="position: absolute; width: 0px; height: 0px; overflow: hidden; padding: 0px; border: 0px; margin: 0px;"><div id="MathJax_Font_Test" style="position: absolute; visibility: hidden; top: 0px; left: 0px; width: auto; min-width: 0px; max-width: none; padding: 0px; border: 0px; margin: 0px; white-space: nowrap; text-align: left; text-indent: 0px; text-transform: none; line-height: normal; letter-spacing: normal; word-spacing: normal; font-size: 40px; font-weight: normal; font-style: normal; font-size-adjust: none; font-family: MathJax_Size1, monospace;"></div></div><iframe id="hfcr" src="./Untitled21.ipynb - Colab_files/RotateCookiesPage.html" style="display: none;"></iframe><div class="notebook-vertical colab-left-pane-open" style="position: relative;">
      <!--?lit$050605479$--><colab-skip-link><template shadowrootmode="open"><!----><md-elevated-button class="link" href="#notebook-main" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><md-elevation part="elevation" aria-hidden="true"><template shadowrootmode="open"><!----><span class="shadow"></span></template></md-elevation>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="link" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="link" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><a id="link" class="button" href="https://colab.research.google.com/drive/1SRMnbgb9yKuwM9M4JRgH7FB5Rigi1Y2g#notebook-main"><!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </a>
    </template><!--?lit$050605479$-->Skip to main content</md-elevated-button></template></colab-skip-link>
      <div class="top-floater"><div role="banner">
    <!--?lit$050605479$-->
    <!--?lit$050605479$-->
          <div id="private-outputs-warning" class="header-warning private-outputs-warning" hidden=""><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>info</md-icon>
            <div class="message">
              <!--?lit$050605479$-->This notebook is open with private outputs. Outputs will not be saved. You can disable this in <a href="https://colab.research.google.com/drive/1SRMnbgb9yKuwM9M4JRgH7FB5Rigi1Y2g#" id="private-outputs-notebook-info-link" command="notebook-settings" aria-describedby="private-outputs-notebook-info-link-tooltip">Notebook settings</a><colab-tooltip-trigger aria-hidden="true" for="private-outputs-notebook-info-link" id="private-outputs-notebook-info-link-tooltip"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Open notebook settings</div><!----><!--?--></template>
        </colab-tooltip-trigger>.
            </div>
          <div class="actions"><md-icon-button class="close" title="Close" data-aria-label="Close" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Close">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>close</md-icon>
        </md-icon-button></div></div>
        
    <!--?lit$050605479$-->

    <div id="header" class="horizontal layout" style="">
      <div id="header-background"><div></div></div>
      <div id="header-content">
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><div id="header-logo">
              <!--?lit$050605479$--> <!--?lit$050605479$--><a href="https://drive.google.com/drive/search?q=owner%3Ame%20(type%3Aapplication%2Fvnd.google.colaboratory%20%7C%7C%20type%3Aapplication%2Fvnd.google.colab)&amp;authuser=0" aria-label="View in Google Drive">
        <!--?lit$050605479$--><md-icon class="colab-large-icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$-->
      <g id="colab-logo">
        <path d="M4.54,9.46,2.19,7.1a6.93,6.93,0,0,0,0,9.79l2.36-2.36A3.59,3.59,0,0,1,4.54,9.46Z" style="fill:var(--colab-logo-dark)"></path>
        <path d="M2.19,7.1,4.54,9.46a3.59,3.59,0,0,1,5.08,0l1.71-2.93h0l-.1-.08h0A6.93,6.93,0,0,0,2.19,7.1Z" style="fill:var(--colab-logo-light)"></path>
        <path d="M11.34,17.46h0L9.62,14.54a3.59,3.59,0,0,1-5.08,0L2.19,16.9a6.93,6.93,0,0,0,9,.65l.11-.09" style="fill:var(--colab-logo-light)"></path>
        <path d="M12,7.1a6.93,6.93,0,0,0,0,9.79l2.36-2.36a3.59,3.59,0,1,1,5.08-5.08L21.81,7.1A6.93,6.93,0,0,0,12,7.1Z" style="fill:var(--colab-logo-light)"></path>
        <path d="M21.81,7.1,19.46,9.46a3.59,3.59,0,0,1-5.08,5.08L12,16.9A6.93,6.93,0,0,0,21.81,7.1Z" style="fill:var(--colab-logo-dark)"></path>
      </g></svg></md-icon>
      </a><!--?-->
            </div>
        <div id="header-doc-toolbar" class="flex">
          <div id="document-info">
            <!--?lit$050605479$--> <!--?lit$050605479$--><md-icon class="file-location-icon" id="file-type" aria-hidden="true" title="Notebook stored in Google Drive"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->
      <svg viewBox="0 0 192 192">
        <path d="M128.33,122l7.59,26.17l19.89,21.42c0,0,0,0,0,0v0c2.69-1.55,4.98-3.8,6.59-6.59l18.48-32 c1.61-2.78,2.41-5.89,2.41-9l-28.38-5.5L128.33,122z" fill="#EA4335"></path>
        <path d="M123.48,18.41c-2.69-1.55-5.78-2.41-9-2.41H77.53c-3.2,0-6.32,0.88-9,2.41l0,0l7.96,26.81l19.44,20.64 L96,66l0,0l19.58-20.89L123.48,18.41C123.48,18.41,123.48,18.41,123.48,18.41C123.48,18.41,123.48,18.41,123.48,18.41z" fill="#188038"></path>
        <path d="M63.67,122l-28.33-6.5L8.72,122c0,3.1,0.8,6.2,2.4,8.99L29.6,163c1.61,2.78,3.9,5.03,6.59,6.59 l19.59-20.18L63.67,122L63.67,122z" fill="#1967D2"></path>
        <path d="M155.47,69l-25.4-44c-1.61-2.79-3.9-5.04-6.59-6.59L96,66l32.33,56h54.95c0-3.11-0.8-6.21-2.41-9 L155.47,69z" fill="#FBBC04"></path><path d="M128.33,122H63.67l-27.48,47.59c2.69,1.55,5.78,2.41,9,2.41h101.61c3.22,0,6.31-0.86,9-2.41L128.33,122z" fill="#4285F4"></path>
        <path d="M96,66L68.53,18.41c-2.69,1.55-4.97,3.79-6.58,6.57l-50.83,88.05c-1.6,2.78-2.4,5.88-2.4,8.97h54.95L96,66 z" fill="#34A853"></path>
      </svg></md-icon>
    <input id="doc-name" class="doc-name" maxlength="259" autocomplete="off" aria-label="Notebook name" command="rename" aria-describedby="doc-name-tooltip" style="width: 136.988px;"><colab-tooltip-trigger aria-hidden="true" for="doc-name" id="doc-name-tooltip"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Rename notebook</div><!----><!--?--></template>
        </colab-tooltip-trigger><colab-input-sizer aria-hidden="true" style="left: -1000%; position: absolute; font-family: &quot;Google Sans&quot;, Roboto, Noto, sans-serif; font-size: 18px; font-weight: 400; letter-spacing: normal; padding-left: 3px; padding-right: 4px; white-space: pre;">Untitled21.ipynb_</colab-input-sizer>
            <!--?lit$050605479$-->
                  <md-icon-button id="star-icon" command="toggle-star" aria-describedby="star-icon-tooltip" data-aria-label="Star" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Star">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
                    <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>star</md-icon>
                  </md-icon-button><colab-tooltip-trigger aria-hidden="true" for="star-icon" id="star-icon-tooltip"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Star notebook in Google Drive</div><!----><!--?--></template>
        </colab-tooltip-trigger>
                
            <!--?lit$050605479$--><colab-last-saved-indicator aria-live="polite" aria-atomic="true"><template shadowrootmode="open"><!----><md-icon-button id="button" data-aria-label="All changes saved" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="All changes saved">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->cloud_done</md-icon></md-icon-button><colab-tooltip-trigger aria-hidden="true" for="button" id="button-tooltip" message="All changes saved"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->All changes saved</div><!----><!--?--></template>
        </colab-tooltip-trigger></template></colab-last-saved-indicator>
          </div>
        <div class="menubar-wrapper"><div><!----><div id="top-menubar" class="goog-menubar format-lightborder" role="menubar" style="user-select: none;" tabindex="0"><!--?lit$050605479$--><div class="goog-menu-button goog-inline-block" id="file-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$050605479$-->File</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div><div class="goog-menu-button goog-inline-block" id="edit-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$050605479$-->Edit</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div><div class="goog-menu-button goog-inline-block" id="view-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$050605479$-->View</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div><div class="goog-menu-button goog-inline-block" id="insert-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$050605479$-->Insert</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div><div class="goog-menu-button goog-inline-block" id="runtime-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$050605479$-->Runtime</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div><div class="goog-menu-button goog-inline-block" id="tools-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$050605479$-->Tools</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div><div class="goog-menu-button goog-inline-block" id="help-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$050605479$-->Help</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div></div></div></div></div>
        <div id="header-right">
          <!--?lit$050605479$-->
    <colab-collaborator-bar id="collaborator-bar"><template shadowrootmode="open"><!----> <div class="collaborator-bar">
      <!--?lit$050605479$-->
      <!--?lit$050605479$-->
    </div></template></colab-collaborator-bar>
  
          <!--?lit$050605479$--> <md-icon-button id="comments" command="open-comments-thread" data-aria-label="Open comments pane" aria-describedby="comments-tooltip" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Open comments pane">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
                <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>comment</md-icon>
              </md-icon-button><colab-tooltip-trigger aria-hidden="true" for="comments" id="comments-tooltip"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Open comments pane</div><!----><!--?--></template>
        </colab-tooltip-trigger>
          <!--?lit$050605479$--> <md-icon-button id="settings-cog" command="preferences" data-aria-label="Open settings" aria-describedby="settings-cog-tooltip" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Open settings">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
                <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>settings</md-icon>
              </md-icon-button><colab-tooltip-trigger aria-hidden="true" for="settings-cog" id="settings-cog-tooltip"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Open settings</div><!----><!--?--></template>
        </colab-tooltip-trigger>
          <!--?lit$050605479$--> <md-filled-tonal-button id="share-toolbar-button" command="share" aria-describedby="share-toolbar-button-tooltip" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><md-elevation part="elevation" aria-hidden="true"><template shadowrootmode="open"><!----><span class="shadow"></span></template></md-elevation>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
                <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->people</md-icon>
                <!--?lit$050605479$-->Share
              </md-filled-tonal-button><colab-tooltip-trigger aria-hidden="true" for="share-toolbar-button" id="share-toolbar-button-tooltip"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Share notebook</div><!----><!--?--></template>
        </colab-tooltip-trigger>
          <!--?lit$050605479$--> <md-icon-button class="show-chat-button" id="show-chat-button" command="show-chat" data-aria-label="Show Gemini" aria-describedby="show-chat-button-tooltip" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Show Gemini">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
                <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
              </md-icon-button><colab-tooltip-trigger aria-hidden="true" for="show-chat-button" id="show-chat-button-tooltip"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Show Gemini</div><!----><!--?--></template>
        </colab-tooltip-trigger>
          <div class="header-onegoogle-container"><div class="onegoogle"><div class="gb_Fa gb_Jd gb_2d gb_Wc gb_H" id="gb" style="background-color: transparent;"><div class="gb_Cd gb_Zd gb_xd" ng-non-bindable="" data-ogsr-up="" style="padding:0;height:auto;display:block"><div class="gb_Qe" style="display:block"><div class="gb_3c"></div><div class="gb_z gb_cd gb_Mf gb_0"><div class="gb_D gb_jb gb_Mf gb_0"><a class="gb_B gb_Za gb_0" aria-expanded="false" aria-label="Google Account: Maryam Sayed  
(maryamsayed207@gmail.com)" href="https://accounts.google.com/SignOutOptions?hl=en&amp;continue=https://colab.research.google.com/&amp;ec=GBRAqQM" tabindex="0" role="button"><img class="gb_P gbii" src="./Untitled21.ipynb - Colab_files/unnamed.jpg" srcset="https://lh3.googleusercontent.com/ogw/AF2bZyiHzNLMQexCE5TuxWfFF-dIGnyf-5pxvZt94XxlsVfhE-g=s32-c-mo 1x, https://lh3.googleusercontent.com/ogw/AF2bZyiHzNLMQexCE5TuxWfFF-dIGnyf-5pxvZt94XxlsVfhE-g=s64-c-mo 2x " alt="" aria-hidden="true" data-noaft=""><div class="gb_Q gb_R" aria-hidden="true"><svg class="gb_Ka" height="14" viewBox="0 0 14 14" width="14" xmlns="http://www.w3.org/2000/svg"><circle class="gb_La" cx="7" cy="7" r="7"></circle><path class="gb_Na" d="M6 10H8V12H6V10ZM6 2H8V8H6V2Z"></path></svg></div></a></div></div></div><div aria-hidden="true" style="overflow: hidden; position: absolute; top: 0px; visibility: hidden; width: 436px; z-index: 991; height: 0px; margin-top: 57px; right: 0px; margin-right: 4px;"><iframe role="presentation" frameborder="0" scrolling="no" name="account" src="./Untitled21.ipynb - Colab_files/saved_resource.html" style="height: 100%; width: 100%; color-scheme: light; visibility: hidden;"></iframe></div><div style="overflow: hidden; position: absolute; top: 0px; visibility: hidden; width: 420px; z-index: 991; height: 280px; margin-top: 70px; right: 0px; margin-right: 25px;"></div></div></div><script nonce="">this.gbar_=this.gbar_||{};(function(_){var window=this;
try{
_.qd=function(a,b,c){if(!a.j)if(c instanceof Array)for(var d of c)_.qd(a,b,d);else{d=(0,_.z)(a.C,a,b);const e=a.v+c;a.v++;b.dataset.eqid=e;a.B[e]=d;b&&b.addEventListener?b.addEventListener(c,d,!1):b&&b.attachEvent?b.attachEvent("on"+c,d):a.o.log(Error("D`"+b))}};
}catch(e){_._DumpException(e)}
try{
var sd=document.querySelector(".gb_J .gb_B"),td=document.querySelector("#gb.gb_Sc");sd&&!td&&_.qd(_.cd,sd,"click");
}catch(e){_._DumpException(e)}
try{
_.Yg=function(a){if(a.v)return a.v;for(const b in a.i)if(a.i[b].fa()&&a.i[b].B())return a.i[b];return null};_.Zg=function(a,b){a.i[b.J()]=b};var $g=new class extends _.Q{constructor(){var a=_.Oc;super();this.B=a;this.v=null;this.o={};this.C={};this.i={};this.j=null}A(a){this.i[a]&&(_.Yg(this)&&_.Yg(this).J()==a||this.i[a].R(!0))}Pa(a){this.j=a;for(const b in this.i)this.i[b].fa()&&this.i[b].Pa(a)}fc(a){return a in this.i?this.i[a]:null}};_.fd("dd",$g);
}catch(e){_._DumpException(e)}
try{
_.qi=function(a,b){return _.K(a,36,b)};
}catch(e){_._DumpException(e)}
try{
var ri=document.querySelector(".gb_z .gb_B"),si=document.querySelector("#gb.gb_Sc");ri&&!si&&_.qd(_.cd,ri,"click");
}catch(e){_._DumpException(e)}
})(this.gbar_);
// Google Inc.
</script></div></div>
        </div>
      </div>
    </div>
  </div></div><colab-notebook-toolbar id="top-toolbar" class="horizontal layout center noshrink toolbar-above-left-pane"><!----> <!--?lit$050605479$--> <colab-toolbar-button icon="search" id="toolbar-show-command-palette" command="show-command-palette"><template shadowrootmode="open"><!----><md-text-button id="button" data-aria-disabled="false" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$-->
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
        <!--?lit$050605479$--><md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->search</md-icon>
        <span class="button-content"><slot></slot></span>
        <!--?lit$050605479$--><span class="screenreader-only"><!--?lit$050605479$-->Show command palette <!--?lit$050605479$-->Ctrl+Shift+P</span>
      </md-text-button>
      <!--?lit$050605479$--> <colab-tooltip-trigger for="button" aria-hidden="true" id="tooltip" message="Show command palette" shortcut="Ctrl+Shift+P"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Show command palette (Ctrl+Shift+P)</div><!----><!--?--></template>
          </colab-tooltip-trigger><!--?--></template>
            <!--?lit$050605479$-->Commands
          </colab-toolbar-button>
          <span class="colab-separator"></span>
    <!--?lit$050605479$-->
          <colab-toolbar-button command="insert-cell-below" icon="add" id="toolbar-add-code"><template shadowrootmode="open"><!----><md-text-button id="button" data-aria-disabled="false" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$-->
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
        <!--?lit$050605479$--><md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->add</md-icon>
        <span class="button-content"><slot></slot></span>
        <!--?lit$050605479$--><span class="screenreader-only"><!--?lit$050605479$-->Insert code cell below <!--?lit$050605479$-->Ctrl+M B</span>
      </md-text-button>
      <!--?lit$050605479$--> <colab-tooltip-trigger for="button" aria-hidden="true" id="tooltip" message="Insert code cell below" shortcut="Ctrl+M B"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Insert code cell below (Ctrl+M B)</div><!----><!--?--></template>
          </colab-tooltip-trigger><!--?--></template>
            <!--?lit$050605479$-->Code
          </colab-toolbar-button>
          <!--?lit$050605479$-->
          <colab-toolbar-button command="add-text" icon="add" id="toolbar-add-text"><template shadowrootmode="open"><!----><md-text-button id="button" data-aria-disabled="false" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$-->
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
        <!--?lit$050605479$--><md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->add</md-icon>
        <span class="button-content"><slot></slot></span>
        <!--?lit$050605479$--><span class="screenreader-only"><!--?lit$050605479$-->Add text cell <!--?lit$050605479$--></span>
      </md-text-button>
      <!--?lit$050605479$--> <colab-tooltip-trigger for="button" aria-hidden="true" id="tooltip" message="Add text cell" shortcut=""><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Add text cell</div><!----><!--?--></template>
          </colab-tooltip-trigger><!--?--></template>
            <!--?lit$050605479$-->Text
          </colab-toolbar-button>
        
    <!--?lit$050605479$-->
    <!--?lit$050605479$-->
    <!--?lit$050605479$-->
    <!--?lit$050605479$--> <span class="collapsed-options">
          <colab-last-saved-indicator aria-live="polite" aria-atomic="true"><template shadowrootmode="open"><!----><md-icon-button id="button" data-aria-label="All changes saved" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="All changes saved">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->cloud_done</md-icon></md-icon-button><colab-tooltip-trigger aria-hidden="true" for="button" id="button-tooltip" message="All changes saved"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->All changes saved</div><!----><!--?--></template>
        </colab-tooltip-trigger></template></colab-last-saved-indicator>
        </span>

    <span class="flex"></span>
    <!--?lit$050605479$--><colab-connect-warning-button><template shadowrootmode="open"><!----><!--?lit$050605479$--><!--?--><!--?--></template></colab-connect-warning-button>
    <!--?lit$050605479$--><!--?lit$050605479$--><colab-connect-button><template shadowrootmode="open"><!----> <!--?lit$050605479$--><md-icon-button aria-describedby="agent-mode-indicator-tooltip" class="agent-mode-indicator" id="agent-mode-indicator" href="https://research.google.com/colaboratory/faq.html#dsa-autonomous-execution" target="_blank" data-aria-label="Agent mode enabled. Click to learn more." value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><div id="button" class="icon-button  standard ">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="link" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple for="link" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$-->
      <a class="link" id="link" href="https://research.google.com/colaboratory/faq.html#dsa-autonomous-execution" target="_blank" aria-label="Agent mode enabled. Click to learn more.">
        <!--?lit$050605479$--><span class="touch"></span>
      </a>
    
  </div></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>shield_person</md-icon></md-icon-button>
      <colab-tooltip-trigger for="agent-mode-indicator" id="agent-mode-indicator-tooltip" aria-hidden="true" message="Agent mode enabled. Click to learn more."><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Agent mode enabled. Click to learn more.</div><!----><!--?--></template>
      </colab-tooltip-trigger> <!--?lit$050605479$--><md-icon-button id="connect-icon" class="icon-okay" data-aria-label="Focus the last run cell" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Focus the last run cell">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
            <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->done</md-icon>
          </md-icon-button>
          <colab-tooltip-trigger for="connect-icon" id="connect-icon-tooltip" aria-hidden="true" message="Focus the last run cell"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Focus the last run cell</div><!----><!--?--></template>
          </colab-tooltip-trigger>
      <colab-toolbar-button id="connect" tooltipid="colab-connect-tooltip" tooltiptext="Connected to
Python 3 Google Compute Engine backend
RAM: 1.48 GB/12.67 GB
Disk: 36.94 GB/107.72 GB"><template shadowrootmode="open"><!----><md-text-button id="button" value="" data-aria-disabled="false"><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$-->
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
        <!--?lit$050605479$-->
        <span class="button-content"><slot></slot></span>
        <!--?lit$050605479$--><span class="screenreader-only"><!--?lit$050605479$-->Connected to
Python 3 Google Compute Engine backend
RAM: 1.48 GB/12.67 GB
Disk: 36.94 GB/107.72 GB <!--?lit$050605479$--></span>
      </md-text-button>
      <!--?lit$050605479$--> <colab-tooltip-trigger for="button" aria-hidden="true" id="colab-connect-tooltip" message="Connected to
Python 3 Google Compute Engine backend
RAM: 1.48 GB/12.67 GB
Disk: 36.94 GB/107.72 GB" shortcut=""><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Connected to</div><!----><!----><div><!--?lit$050605479$-->Python 3 Google Compute Engine backend</div><!----><!----><div><!--?lit$050605479$-->RAM: 1.48 GB/12.67 GB</div><!----><!----><div><!--?lit$050605479$-->Disk: 36.94 GB/107.72 GB</div><!----><!--?--></template>
          </colab-tooltip-trigger><!--?--></template>
        <!--?lit$050605479$--> <div id="connect-button-resource-display">
        <!--?lit$050605479$--><colab-usage-sparkline class="ram" label="RAM"><template shadowrootmode="open"><!---->
      <div class="label"><!--?lit$050605479$-->RAM</div>
      <!--?lit$050605479$-->
      <canvas height="14" width="20"></canvas>
    </template></colab-usage-sparkline>
        <!--?lit$050605479$--><colab-usage-sparkline class="disks" label="Disk"><template shadowrootmode="open"><!---->
      <div class="label"><!--?lit$050605479$-->Disk</div>
      <!--?lit$050605479$-->
      <canvas height="14" width="20"></canvas>
    </template></colab-usage-sparkline>
      </div>
      </colab-toolbar-button>
      <!--?lit$050605479$--> <md-icon-button id="connect-dropdown" data-aria-expanded="false" data-aria-haspopup="menu" data-aria-label="Additional connection options" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Additional connection options" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>arrow_drop_down</md-icon>
      </md-icon-button>
      <colab-tooltip-trigger for="connect-dropdown" id="connect-dropdown-tooltip" aria-hidden="true" message="Additional connection options"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Additional connection options</div><!----><!--?--></template>
      </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?--></template></colab-connect-button><!--?-->
    <!--?lit$050605479$-->
    <span class="collapsed-options">
      <!--?lit$050605479$--><span class="colab-separator"></span>
      <!--?lit$050605479$--> <md-icon-button id="share-button-toolbar" command="share" data-aria-label="Share notebook" aria-describedby="share-button-toolbar-tooltip" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Share notebook">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
            <md-icon filled="" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->people</md-icon>
          </md-icon-button><colab-tooltip-trigger aria-hidden="true" for="share-button-toolbar" id="share-button-toolbar-tooltip"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Share notebook</div><!----><!--?--></template>
        </colab-tooltip-trigger><md-icon-button id="settings-button-toolbar" command="preferences" data-aria-label="Open settings" aria-describedby="settings-button-toolbar-tooltip" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Open settings">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon filled="" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>settings</md-icon>
      </md-icon-button><colab-tooltip-trigger aria-hidden="true" for="settings-button-toolbar" id="settings-button-toolbar-tooltip"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Open settings</div><!----><!--?--></template>
        </colab-tooltip-trigger>
      <!--?lit$050605479$--> <md-icon-button class="show-chat-button" id="show-chat-button-toolbar" command="show-chat" data-aria-label="Show Gemini" aria-describedby="show-chat-button-toolbar-tooltip" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Show Gemini">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
            <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
          </md-icon-button><colab-tooltip-trigger aria-hidden="true" for="show-chat-button-toolbar" id="show-chat-button-toolbar-tooltip"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Show Gemini</div><!----><!--?--></template>
        </colab-tooltip-trigger>
    </span>
    <span class="colab-separator"></span>
    <!--?lit$050605479$--><md-icon-button toggle="" command="toggle-header" id="toggle-header-button" data-aria-label="Toggle header visibility" aria-describedby="toggle-header-button-tooltip" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button standard" aria-label="Toggle header visibility" aria-pressed="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
    <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>expand_less</md-icon>
    <md-icon slot="selected" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>expand_more</md-icon>
  </md-icon-button><colab-tooltip-trigger aria-hidden="true" for="toggle-header-button" id="toggle-header-button-tooltip"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Toggle header visibility</div><!----><!--?--></template>
        </colab-tooltip-trigger><!--?--></colab-notebook-toolbar><div class="notebook-horizontal">
        <!--?lit$050605479$--><colab-left-pane role="complementary" aria-label="left pane" class="colab-left-pane-open"><!----><div class="colab-left-pane-nib layout vertical" role="toolbar" aria-orientation="vertical">
        <div class="left-pane-top"><!----><div class="left-pane-button">
        <!--?lit$050605479$--><md-icon-button toggle="" command="show-toc-pane" data-aria-label="Table of contents" title="Table of contents" value="" tabindex="-1"><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Table of contents" aria-pressed="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->format_list_bulleted</md-icon>
    </md-icon-button> <!--?lit$050605479$-->
      </div><!----><div class="left-pane-button">
        <!--?lit$050605479$--><md-icon-button toggle="" command="find" data-aria-label="Find and replace" title="Find and replace" value="" tabindex="-1"><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Find and replace" aria-pressed="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->find_in_page</md-icon>
    </md-icon-button> <!--?lit$050605479$-->
      </div><!----><div class="left-pane-button">
        <!--?lit$050605479$--><md-icon-button toggle="" command="show-variables" data-aria-label="Variables" title="Variables" value="" tabindex="-1"><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Variables" aria-pressed="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$-->
      <path d="M4.51,9.44V6.08c0-1.34.37-1.85,1.6-2.17l.22-.06V3.13l-.27,0-.44,0a4.46,4.46,0,0,0-2.2.59,2.78,2.78,0,0,0-1,2.51V9.74c0,1.26-.26,1.61-1.49,2L0,12l.94.29c1.21.38,1.49.75,1.49,2v3.5a2.94,2.94,0,0,0,1,2.6,4.39,4.39,0,0,0,2.14.56l.46,0,.27,0v-.72l-.22-.06c-1.24-.32-1.6-.81-1.6-2.17V14.58c0-1.43-.3-2.13-1.25-2.57C4.2,11.57,4.51,10.87,4.51,9.44Z"></path>
      <path d="M23.06,11.71c-1.22-.36-1.49-.71-1.49-2l0-3.5a3,3,0,0,0-1-2.6,4.38,4.38,0,0,0-2.14-.56l-.46,0-.27,0v.72l.22.06c1.24.32,1.6.81,1.6,2.17V9.44c0,1.44.3,2.13,1.25,2.57-1,.44-1.25,1.14-1.25,2.57v3.36c0,1.34-.37,1.85-1.6,2.17l-.22.06v.72l.27,0,.44,0a4.47,4.47,0,0,0,2.2-.59,2.82,2.82,0,0,0,1-2.51V14.28c0-1.26.26-1.61,1.49-2L24,12Z"></path>
      <path d="M15.16,8.22a.88.88,0,0,1,.46.16,1.25,1.25,0,0,0,.69.2h0A1,1,0,0,0,17,8.23a1.06,1.06,0,0,0,.24-.8,1.1,1.1,0,0,0-1.15-1h0c-1,0-1.73.64-3,2.57l-.12-.51c-.28-1.36-.56-2-1.39-2h0A8,8,0,0,0,9,7.08l-.47.16.16.91L9.41,8a3.22,3.22,0,0,1,.73-.14c.34,0,.43,0,.71,1.2l.56,2.47L9.76,13.82a3.6,3.6,0,0,1-.8.88.9.9,0,0,1-.38-.13,1.83,1.83,0,0,0-.88-.28,1,1,0,0,0-1,1.06A1.15,1.15,0,0,0,8,16.53c.85,0,1.35-.35,2.24-1.55l1.49-2,.46,1.88c.23,1,.46,1.66,1.53,1.66s1.66-.75,2.81-2.53l.17-.26-.81-.48-.16.2-.25.34-.19.25c-.45.57-.62.73-.76.73s-.28-.4-.34-.63l-.67-2.83a4.2,4.2,0,0,1-.15-.79C13.84,9.78,14.74,8.22,15.16,8.22Z"></path></svg></md-icon>
    </md-icon-button> <!--?lit$050605479$-->
      </div><!----><div class="left-pane-button">
        <!--?lit$050605479$--><md-icon-button toggle="" command="open-user-secrets" data-aria-label="Secrets" title="Secrets" value="" tabindex="-1"><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Secrets" aria-pressed="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->vpn_key</md-icon>
    </md-icon-button> <!--?lit$050605479$-->
      </div><!----><div class="left-pane-button">
        <!--?lit$050605479$--><md-icon-button toggle="" command="show-files" data-aria-label="Files" title="Files" value="" selected=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button standard selected" aria-label="Files" aria-pressed="true">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="icon icon--selected"><slot name="selected"><slot></slot></slot></span>
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->folder</md-icon>
    </md-icon-button> <!--?lit$050605479$-->
      </div></div>
        <div class="left-pane-bottom"><!----><div class="left-pane-button">
        <!--?lit$050605479$--><md-icon-button command="snippets" data-aria-label="Code snippets" title="Code snippets" value="" tabindex="-1"><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code snippets">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->code</md-icon>
    </md-icon-button> <!--?lit$050605479$-->
      </div><!----><div class="left-pane-button">
        <!--?lit$050605479$--><md-icon-button command="show-terminal" data-aria-label="Terminal" title="Terminal" value="" tabindex="-1"><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Terminal">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->terminal</md-icon>
    </md-icon-button> <!--?lit$050605479$-->
      </div></div>
      </div><colab-resizer class="ew-resize" style="width: 218px;">
          <div class="resizer-contents">
            <div class="colab-left-pane-header layout horizontal noshrink">
              <h3 class="left-pane-content-title">Files</h3>
              <!--?lit$050605479$--><md-icon-button class="colab-left-pane-move" data-aria-label="Move left pane to a tab" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Move left pane to a tab">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>tab</md-icon>
    </md-icon-button> <!--?lit$050605479$--><md-icon-button class="colab-left-pane-close" data-aria-label="Close left pane" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Close left pane">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>close</md-icon>
    </md-icon-button>
            </div>
            <div class="left-pane-container"><colab-file-browser class="layout vertical"><colab-file-tree><!----> <!--?lit$050605479$--><colab-agent-promo-banner><template shadowrootmode="open"><!----><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <div><!--?lit$050605479$-->Analyze your files with code written by Gemini</div>
      <md-text-button value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$-->
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
        <!--?lit$050605479$-->Upload
      </md-text-button></template>
            </colab-agent-promo-banner>
        <div class="file-tree-buttons">
          <label for="file-tree-upload-input">
            <md-icon-button class="colab-icon file-tree-upload-button" title="Upload to session storage" data-aria-label="Upload to session storage" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Upload to session storage">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
              <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>upload_file</md-icon>
            </md-icon-button>
          </label>
          <input id="file-tree-upload-input" type="file" multiple="">
          <md-icon-button class="file-tree-refresh" title="Refresh" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard ">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
            <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>refresh</md-icon>
          </md-icon-button>
          <md-icon-button toggle="" class="mount-drive-button" title="Mount Drive" data-aria-label="Mount Drive" aria-label-selected="Unmount Drive" style="display: flex;" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Mount Drive" aria-pressed="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
            <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$-->
    <path d="M20,6H12L10,4H4A2,2,0,0,0,2,6V18a2,2,0,0,0,2,2H20a2,2,0,0,0,2-2V8A2,2,0,0,0,20,6ZM13.57,9.32,13,8.4l.34-.6h3.11l3.69,6.5H16.38M12.11,17l-.67,1.2h-1L9,15.42,12.72,9l2,3.46h0M19.3,18.2H12.09l.67-1.2,1.15-2h6.64l.34.6Z"></path></svg></md-icon>
            <md-icon slot="selected" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$-->
    <path d="M12.72,9l2,3.46h0l-.26.47,2,2h4.1l.34.6L19.45,18l1.69,1.69A2,2,0,0,0,22,18V8a2,2,0,0,0-2-2H12L10,4H5.5l6.4,6.4Zm.66-1.17h3.11l3.69,6.5H16.38l-2.81-5L13,8.4Z"></path>
    <path d="M22.19,22.19,1.81,1.81.4,3.22,2.25,5.07A2,2,0,0,0,2,6V18a2,2,0,0,0,2,2H17.17l3.61,3.61Zm-11.73-4L9,15.42l1.3-2.26,2.35,2.36.17.17L12.11,17l-.67,1.2Zm1.63,0,.67-1.2.51-.9,2.1,2.1Z"></path></svg></md-icon>
          </md-icon-button>
          <md-icon-button toggle="" id="hidden-files-toggle" data-aria-label="Show hidden files" aria-label-selected="Hide hidden files" title="Show hidden files" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Show hidden files" aria-pressed="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
            <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>visibility_off</md-icon>
            <md-icon slot="selected" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>visibility</md-icon>
          </md-icon-button>
        </div>
        <div class="parent-link"><div class="file-title-row">
          <!--?lit$050605479$-->
                <div class="file-icon colab-icon" style="margin-left: 0px;"></div>
              
          <md-icon class="file-icon colab-icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->folder_open</md-icon>
          <span class="file-tree-name" title="Up one level">
            <!--?lit$050605479$-->..
          </span>
          <input class="file-tree-name-input" value="..">
          <md-icon-button class="file-item-menu" data-aria-expanded="false" data-aria-haspopup="menu" data-aria-label="More actions for file: .." value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="More actions for file: .." aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_vert</md-icon></md-icon-button>
        </div></div>
        <div class="files-root"><colab-file-view filename="content" draggable="true"><!----><!--?lit$050605479$--><!--?--><!--?lit$050605479$-->
        <div class="child-files"><colab-file-view filename="sample_data" class="collapsed" draggable="true"><!----><!--?lit$050605479$-->
        <div class="file-title-row">
          <!--?lit$050605479$--> <md-icon class="file-icon colab-icon directory-icon" style="margin-left: 0px;" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>arrow_drop_down</md-icon>
          <md-icon class="file-icon colab-icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->folder</md-icon>
          <span class="file-tree-name" title="sample_data">
            <!--?lit$050605479$-->sample_data
          </span>
          <input class="file-tree-name-input" value="sample_data">
          <md-icon-button class="file-item-menu" data-aria-expanded="false" data-aria-haspopup="menu" data-aria-label="More actions for folder: sample_data" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="More actions for folder: sample_data" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_vert</md-icon></md-icon-button>
        </div>
      <!--?lit$050605479$-->
        <div class="child-files"></div>
        <div class="overflow-ellipsis" title="Directory is too large to display all files." style="margin-left: 0px;">
          …
        </div>
      <!--?--></colab-file-view><colab-file-view filename="201904-fordgobike-tripdata.csv" draggable="true"><!----><!--?lit$050605479$-->
        <div class="file-title-row">
          <!--?lit$050605479$-->
                <div class="file-icon colab-icon" style="margin-left: 0px;"></div>
              
          <md-icon class="file-icon colab-icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->draft</md-icon>
          <span class="file-tree-name" title="201904-fordgobike-tripdata.csv (49.14M) 
Last modified Thu Mar 13 2025 00:54:50 GMT+0200 (Eastern European Standard Time)">
            <!--?lit$050605479$-->201904-fordgobike-tripdata.csv
          </span>
          <input class="file-tree-name-input" value="201904-fordgobike-tripdata.csv">
          <md-icon-button class="file-item-menu" data-aria-expanded="false" data-aria-haspopup="menu" data-aria-label="More actions for file: 201904-fordgobike-tripdata.csv" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="More actions for file: 201904-fordgobike-tripdata.csv" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_vert</md-icon></md-icon-button>
        </div>
      <!--?lit$050605479$--><!--?--><!--?--></colab-file-view><colab-file-view filename="app.py" draggable="true"><!----><!--?lit$050605479$-->
        <div class="file-title-row">
          <!--?lit$050605479$-->
                <div class="file-icon colab-icon" style="margin-left: 0px;"></div>
              
          <md-icon class="file-icon colab-icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->draft</md-icon>
          <span class="file-tree-name" title="app.py (1K) 
Last modified Thu Mar 13 2025 01:31:11 GMT+0200 (Eastern European Standard Time)">
            <!--?lit$050605479$-->app.py
          </span>
          <input class="file-tree-name-input" value="app.py">
          <md-icon-button class="file-item-menu" data-aria-expanded="false" data-aria-haspopup="menu" data-aria-label="More actions for file: app.py" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="More actions for file: app.py" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_vert</md-icon></md-icon-button>
        </div>
      <!--?lit$050605479$--><!--?--><!--?--></colab-file-view></div>
        <div class="overflow-ellipsis" title="Directory is too large to display all files." style="margin-left: -20px;">
          …
        </div>
      <!--?--></colab-file-view></div>
        <div class="files-drag-to-upload layout horizontal">
          <md-icon class="layout noshrink" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>upload_file</md-icon>
          <div> <!--?lit$050605479$-->Drop files to upload them to session storage. </div>
        </div>
        <div class="files-uploading"></div>
        <div class="colab-usage-bar-container"><colab-usage-bar aria-describedby="file-browser-disk-display-kernel-tooltip" id="file-browser-disk-display-kernel" class="file-browser-disk-display usage-bar-with-suffix" tabindex="0" style="display: flex;"><template shadowrootmode="open"><!---->
        <div class="header">
          <div><!--?lit$050605479$-->Disk </div>
          <div class="suffix"><!--?lit$050605479$-->70.77 GB available</div>
        </div>
        <!--?lit$050605479$-->
      <div class="progress-container">
        <md-linear-progress class="  " value="0.34297878627664835"><template shadowrootmode="open"><!---->
      <div role="progressbar" aria-valuemin="0" class="progress   " aria-valuemax="1" aria-valuenow="0.34297878627664835"><!--?lit$050605479$-->
      <div class="dots" hidden=""></div>
      <div class="inactive-track" style="transform: scaleX(1);"></div>
      <div class="bar primary-bar" style="transform: scaleX(0.342979);">
        <div class="bar-inner"></div>
      </div>
      <div class="bar secondary-bar">
        <div class="bar-inner"></div>
      </div>
    </div>
    </template></md-linear-progress>
      </div>
    
      </template></colab-usage-bar><colab-tooltip-trigger aria-hidden="true" id="file-browser-disk-display-kernel-tooltip"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Disk: 36.94 GB/107.72 GB</div><!----><!--?--></template></colab-tooltip-trigger></div></colab-file-tree></colab-file-browser></div>
          </div>
        <div class="resizer-thumb"></div></colab-resizer></colab-left-pane>
        <div class="layout vertical grow">
          <colab-tab-layout-container class="layout horizontal grow flexible-tabs"><!----> <div class="layout horizontal tab-pane-parent">
      <!--?lit$050605479$--> <div class="layout vertical tab-pane-parent">
      <!--?lit$050605479$--><colab-tab-pane class="layout vertical grow no-header focused" align="horizontal"><!----> <div class="layout vertical grow">
    <div class="tab-pane-header layout horizontal noshrink">
      <md-tabs><template shadowrootmode="open"><!---->
      <div class="tabs">
        <slot></slot>
      </div>
      <md-divider part="divider"><template shadowrootmode="open"><!----></template></md-divider>
    </template><md-primary-tab noink="" title="" aria-labelledby="tab-title-GS1RS8Auic6r" class="selected-tab" md-tab="" active="" tabindex="0"><template shadowrootmode="open"><!----><div class="button" role="presentation">
      <md-focus-ring part="focus-ring" inward="" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-elevation part="elevation" aria-hidden="true"><template shadowrootmode="open"><!----><span class="shadow"></span></template></md-elevation>
      <md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <div role="presentation" class="content  has-label stacked ">
        <slot name="icon"></slot>
        <slot></slot>
        <!--?lit$050605479$--><div class="indicator"></div>
      </div>
      <!--?lit$050605479$-->
    </div></template>
          <div class="colab-tab-header">
            <span class="colab-tab-title" id="tab-title-GS1RS8Auic6r"><!--?lit$050605479$--><!--?lit$050605479$-->Notebook<!--?--></span>
            <!--?lit$050605479$-->
          </div>
        </md-primary-tab></md-tabs>
      <div class="layout grow"></div>
      <!--?lit$050605479$--> <md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" title="More tab actions" data-aria-label="More tab actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="More tab actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
    <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_horiz</md-icon>
  </md-icon-button>
    </div>
    <div class="layout vertical grow tab-pane-container"> <colab-tab class="layout vertical grow notebook-tab-content selected-tab"><!----> <div class="overflow-flexbox-workaround">
      <colab-shaded-scroller ignore-dom-changes="" role="main" id="notebook-main" class="notebook-container" aria-label="Notebook" tabindex="-1">
        <div class="notebook-scrolling-horizontal-container">
          <div class="notebook-scrolling-horizontal">
            <div class="notebook-content-background">
              <!--?lit$050605479$-->
              <div class="notebook-content ">
                <!--?lit$050605479$--><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div>
                <div class="notebook-cell-list"><div class="cell text" id="cell-FadWD9ovkWdQ" role="region" aria-label="Cell 0: Text cell: Task" style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><div class="text-cell-section-header layout horizontal center"><md-icon-button class="header-section-toggle" title="Collapse 29 child cells under Task (Press &lt;Shift&gt; to also collapse sibling sections)" data-aria-label="Collapse 29 child cells under Task (Press &lt;Shift&gt; to also collapse sibling sections)" style="" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Collapse 29 child cells under Task (Press &lt;Shift&gt; to also collapse sibling sections)">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>keyboard_arrow_down</md-icon></md-icon-button><h1>Task</h1></div>
<p>make analysis and visualization and extract incites</p>
<p>Here is all the data you need:
"201904-fordgobike-tripdata.csv"</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>29 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell text" id="cell-UujWKT0okWt8" role="region" aria-label="Cell 1: Text cell: Data loading" style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><div class="text-cell-section-header layout horizontal center"><md-icon-button class="header-section-toggle" title="Collapse 2 child cells under Data loading (Press &lt;Shift&gt; to also collapse sibling sections)" data-aria-label="Collapse 2 child cells under Data loading (Press &lt;Shift&gt; to also collapse sibling sections)" style="" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Collapse 2 child cells under Data loading (Press &lt;Shift&gt; to also collapse sibling sections)">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>keyboard_arrow_down</md-icon></md-icon-button><h2>Data loading</h2></div>
<h3>Subtask:</h3>
<p>Load the provided CSV file into a pandas DataFrame.</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>2 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell text" id="cell-lz4DEjuIkW94" role="region" aria-label="Cell 2: Text cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><p><strong>Reasoning</strong>:
Load the data into a pandas DataFrame and display the first few rows.</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>0 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling code-has-output" id="cell-F2nK-o7okXNy" role="region" aria-label="Cell 3: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
12:55 AM (29 minutes ago)
executed in 3.599s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->12:55 AM (29 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 3.599s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark" data-lang="notebook-python"><span><span class="mtk18">import</span><span class="mtk1">&nbsp;pandas&nbsp;</span><span class="mtk18">as</span><span class="mtk1">&nbsp;pd</span></span><br><span><span></span></span><br><span><span class="mtk18">try</span><span class="mtk12">:</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;df&nbsp;=&nbsp;pd.read_csv</span><span class="mtk12">(</span><span class="mtk5">'201904-fordgobike-tripdata.csv'</span><span class="mtk12">)</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;display</span><span class="mtk12">(</span><span class="mtk1">df.head</span><span class="mtk12">())</span></span><br><span><span class="mtk18">except</span><span class="mtk1">&nbsp;FileNotFoundError</span><span class="mtk12">:</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"Error:&nbsp;'201904-fordgobike-tripdata.csv'&nbsp;not&nbsp;found</span><span class="mtk5">.&nbsp;Please&nbsp;ensure&nbsp;the&nbsp;file&nbsp;exists&nbsp;in&nbsp;the&nbsp;current&nbsp;dir</span><span class="mtk5">ectory."</span><span class="mtk12">)</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;df&nbsp;=&nbsp;</span><span class="mtk9">None</span><span class="mtk1">&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Indicate&nbsp;failure&nbsp;to&nbsp;load&nbsp;data</span></span><br><span><span class="mtk18">except</span><span class="mtk1">&nbsp;pd.errors.ParserError</span><span class="mtk12">:</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"Error:&nbsp;Could&nbsp;not&nbsp;parse&nbsp;the&nbsp;CSV&nbsp;file.&nbsp;Please&nbsp;check</span><span class="mtk5">&nbsp;the&nbsp;file&nbsp;format."</span><span class="mtk12">)</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;df&nbsp;=&nbsp;</span><span class="mtk9">None</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$050605479$-->Start coding or <span role="button" class="link" tabindex="0">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 3 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div class="outputview" style="height: 365px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals" src="./Untitled21.ipynb - Colab_files/outputframe.html" class="" style="height: 365px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell text" id="cell-Y0TXQDQDkbbF" role="region" aria-label="Cell 4: Text cell: Data exploration" style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><div class="text-cell-section-header layout horizontal center"><md-icon-button class="header-section-toggle" title="Collapse 2 child cells under Data exploration (Press &lt;Shift&gt; to also collapse sibling sections)" data-aria-label="Collapse 2 child cells under Data exploration (Press &lt;Shift&gt; to also collapse sibling sections)" style="" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Collapse 2 child cells under Data exploration (Press &lt;Shift&gt; to also collapse sibling sections)">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>keyboard_arrow_down</md-icon></md-icon-button><h2>Data exploration</h2></div>
<h3>Subtask:</h3>
<p>Explore the loaded dataset to understand its characteristics.</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>2 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell text" id="cell-Y1xkC57_kc3H" role="region" aria-label="Cell 5: Text cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><p><strong>Reasoning</strong>:
Examine the shape, data types, missing values, descriptive statistics, and distributions of key variables in the dataframe.</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>0 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code icon-scrolling code-has-output" id="cell-kHA7VPmfkdHI" role="region" aria-label="Cell 6: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
12:55 AM (29 minutes ago)
executed in 2.423s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->12:55 AM (29 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 2.423s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark" data-lang="notebook-python"><span><span class="mtk8">#&nbsp;Examine&nbsp;the&nbsp;shape&nbsp;of&nbsp;the&nbsp;DataFrame</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"DataFrame&nbsp;Shape:"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;df.shape</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Display&nbsp;data&nbsp;types&nbsp;of&nbsp;each&nbsp;column</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"\nData&nbsp;Types:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;df.dtypes</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Identify&nbsp;and&nbsp;calculate&nbsp;the&nbsp;percentage&nbsp;of&nbsp;missing</span><span class="mtk8">&nbsp;values</span></span><br><span><span class="mtk1">missing_values&nbsp;=&nbsp;df.isnull</span><span class="mtk12">()</span><span class="mtk1">.</span><span class="mtk15">sum</span><span class="mtk12">()</span></span><br><span><span class="mtk1">missing_percentage&nbsp;=&nbsp;</span><span class="mtk12">(</span><span class="mtk1">missing_values&nbsp;/&nbsp;</span><span class="mtk15">len</span><span class="mtk12">(</span><span class="mtk1">df</span><span class="mtk12">))</span><span class="mtk1">&nbsp;*&nbsp;</span><span class="mtk6">100</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"\nMissing&nbsp;Values:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;missing_values</span><span class="mtk12">)</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"\nPercentage&nbsp;of&nbsp;Missing&nbsp;Values:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;missing_percentage</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Summarize&nbsp;descriptive&nbsp;statistics&nbsp;for&nbsp;numerical&nbsp;c</span><span class="mtk8">olumns</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"\nDescriptive&nbsp;Statistics:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;df.describe</span><span class="mtk12">())</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Analyze&nbsp;the&nbsp;distribution&nbsp;of&nbsp;key&nbsp;categorical&nbsp;vari</span><span class="mtk8">ables</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"\nUser&nbsp;Type&nbsp;Distribution:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'user_type'</span><span class="mtk12">]</span><span class="mtk1">.value_counts</span><span class="mtk12">())</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"\nMember&nbsp;Gender&nbsp;Distribution:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'member_gender'</span><span class="mtk12">]</span><span class="mtk1">.value_counts</span><span class="mtk12">())</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Explore&nbsp;the&nbsp;distribution&nbsp;of&nbsp;numerical&nbsp;variables&nbsp;</span><span class="mtk8">(e.g.,&nbsp;duration_sec)</span></span><br><span><span class="mtk18">import</span><span class="mtk1">&nbsp;matplotlib.pyplot&nbsp;</span><span class="mtk18">as</span><span class="mtk1">&nbsp;plt</span></span><br><span><span class="mtk1">plt.figure</span><span class="mtk12">(</span><span class="mtk1">figsize=</span><span class="mtk12">(</span><span class="mtk6">10</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk6">6</span><span class="mtk12">))</span></span><br><span><span class="mtk1">plt.hist</span><span class="mtk12">(</span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'duration_sec'</span><span class="mtk12">],</span><span class="mtk1">&nbsp;bins=</span><span class="mtk6">50</span><span class="mtk12">,</span><span class="mtk1">&nbsp;color=</span><span class="mtk5">'skyblue'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;edgecolor=</span><span class="mtk5">'black'</span><span class="mtk12">)</span></span><br><span><span class="mtk1">plt.title</span><span class="mtk12">(</span><span class="mtk5">'Distribution&nbsp;of&nbsp;Trip&nbsp;Durations'</span><span class="mtk12">)</span></span><br><span><span class="mtk1">plt.xlabel</span><span class="mtk12">(</span><span class="mtk5">'Duration&nbsp;(seconds)'</span><span class="mtk12">)</span></span><br><span><span class="mtk1">plt.ylabel</span><span class="mtk12">(</span><span class="mtk5">'Frequency'</span><span class="mtk12">)</span></span><br><span><span class="mtk1">plt.show</span><span class="mtk12">()</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Examine&nbsp;the&nbsp;relationship&nbsp;between&nbsp;start&nbsp;and&nbsp;end&nbsp;s</span><span class="mtk8">tations</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"\nMost&nbsp;Frequent&nbsp;Start&nbsp;Stations:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'start_station_name'</span><span class="mtk12">]</span><span class="mtk1">.value_counts</span><span class="mtk12">()</span><span class="mtk1">.head</span><span class="mtk12">(</span><span class="mtk6">10</span><span class="mtk12">))</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"\nMost&nbsp;Frequent&nbsp;End&nbsp;Stations:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'end_station_name'</span><span class="mtk12">]</span><span class="mtk1">.value_counts</span><span class="mtk12">()</span><span class="mtk1">.head</span><span class="mtk12">(</span><span class="mtk6">10</span><span class="mtk12">))</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Convert&nbsp;start_time&nbsp;and&nbsp;end_time&nbsp;to&nbsp;datetime&nbsp;obje</span><span class="mtk8">cts</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'start_time'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;pd.to_datetime</span><span class="mtk12">(</span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'start_time'</span><span class="mtk12">])</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'end_time'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;pd.to_datetime</span><span class="mtk12">(</span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'end_time'</span><span class="mtk12">])</span></span><br><span><span class="mtk8">#&nbsp;Explore&nbsp;temporal&nbsp;patterns</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'start_date'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'start_time'</span><span class="mtk12">]</span><span class="mtk1">.dt.date</span></span><br><span><span class="mtk1">trips_per_day&nbsp;=&nbsp;df.groupby</span><span class="mtk12">(</span><span class="mtk5">'start_date'</span><span class="mtk12">)[</span><span class="mtk5">'start_time'</span><span class="mtk12">]</span><span class="mtk1">.count</span><span class="mtk12">()</span></span><br><span><span></span></span><br><span><span class="mtk1">plt.figure</span><span class="mtk12">(</span><span class="mtk1">figsize=</span><span class="mtk12">(</span><span class="mtk6">12</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk6">6</span><span class="mtk12">))</span></span><br><span><span class="mtk1">plt.plot</span><span class="mtk12">(</span><span class="mtk1">trips_per_day.index</span><span class="mtk12">,</span><span class="mtk1">&nbsp;trips_per_day.values</span><span class="mtk12">,</span><span class="mtk1">&nbsp;marker=</span><span class="mtk5">'o'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;linestyle=</span><span class="mtk5">'-'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;color=</span><span class="mtk5">'green'</span><span class="mtk12">)</span></span><br><span><span class="mtk1">plt.title</span><span class="mtk12">(</span><span class="mtk5">'Number&nbsp;of&nbsp;Trips&nbsp;per&nbsp;Day'</span><span class="mtk12">)</span></span><br><span><span class="mtk1">plt.xlabel</span><span class="mtk12">(</span><span class="mtk5">'Date'</span><span class="mtk12">)</span></span><br><span><span class="mtk1">plt.ylabel</span><span class="mtk12">(</span><span class="mtk5">'Number&nbsp;of&nbsp;Trips'</span><span class="mtk12">)</span></span><br><span><span class="mtk1">plt.xticks</span><span class="mtk12">(</span><span class="mtk1">rotation=</span><span class="mtk6">45</span><span class="mtk12">)</span></span><br><span><span class="mtk1">plt.tight_layout</span><span class="mtk12">()</span></span><br><span><span class="mtk1">plt.show</span><span class="mtk12">()</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$050605479$-->Start coding or <span role="button" class="link" tabindex="0">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 6 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div class="outputview" style="height: 1000px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals" src="./Untitled21.ipynb - Colab_files/outputframe(1).html" class="" style="height: 1000px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell text" id="cell-Ri9v37ltkhEX" role="region" aria-label="Cell 7: Text cell: Data cleaning" style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><div class="text-cell-section-header layout horizontal center"><md-icon-button class="header-section-toggle" title="Collapse 4 child cells under Data cleaning (Press &lt;Shift&gt; to also collapse sibling sections)" data-aria-label="Collapse 4 child cells under Data cleaning (Press &lt;Shift&gt; to also collapse sibling sections)" style="" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Collapse 4 child cells under Data cleaning (Press &lt;Shift&gt; to also collapse sibling sections)">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>keyboard_arrow_down</md-icon></md-icon-button><h2>Data cleaning</h2></div>
<h3>Subtask:</h3>
<p>Clean the data by handling missing values and outliers.</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>4 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell text" id="cell-8i3vKvogkh64" role="region" aria-label="Cell 8: Text cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><p><strong>Reasoning</strong>:
Handle missing values in specified columns and outliers in <code>duration_sec</code>.</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>0 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code icon-scrolling code-has-output" id="cell-hPG6Zk-PkiKu" role="region" aria-label="Cell 9: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
12:55 AM (28 minutes ago)
executed in 0.171s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->12:55 AM (28 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 0.171s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark" data-lang="notebook-python"><span><span class="mtk8">#&nbsp;Fill&nbsp;missing&nbsp;station&nbsp;names&nbsp;with&nbsp;'Unknown'</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'start_station_name'</span><span class="mtk12">]</span><span class="mtk1">.fillna</span><span class="mtk12">(</span><span class="mtk5">'Unknown'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;inplace=</span><span class="mtk9">True</span><span class="mtk12">)</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'end_station_name'</span><span class="mtk12">]</span><span class="mtk1">.fillna</span><span class="mtk12">(</span><span class="mtk5">'Unknown'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;inplace=</span><span class="mtk9">True</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Fill&nbsp;missing&nbsp;gender&nbsp;with&nbsp;the&nbsp;mode</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'member_gender'</span><span class="mtk12">]</span><span class="mtk1">.fillna</span><span class="mtk12">(</span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'member_gender'</span><span class="mtk12">]</span><span class="mtk1">.mode</span><span class="mtk12">()[</span><span class="mtk6">0</span><span class="mtk12">],</span><span class="mtk1">&nbsp;inplace=</span><span class="mtk9">True</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Impute&nbsp;missing&nbsp;birth&nbsp;years&nbsp;with&nbsp;the&nbsp;median</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'member_birth_year'</span><span class="mtk12">]</span><span class="mtk1">.fillna</span><span class="mtk12">(</span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'member_birth_year'</span><span class="mtk12">]</span><span class="mtk1">.median</span><span class="mtk12">(),</span><span class="mtk1">&nbsp;inplace=</span><span class="mtk9">True</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Calculate&nbsp;the&nbsp;IQR&nbsp;for&nbsp;duration_sec</span></span><br><span><span class="mtk1">Q1&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'duration_sec'</span><span class="mtk12">]</span><span class="mtk1">.quantile</span><span class="mtk12">(</span><span class="mtk6">0.25</span><span class="mtk12">)</span></span><br><span><span class="mtk1">Q3&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'duration_sec'</span><span class="mtk12">]</span><span class="mtk1">.quantile</span><span class="mtk12">(</span><span class="mtk6">0.75</span><span class="mtk12">)</span></span><br><span><span class="mtk1">IQR&nbsp;=&nbsp;Q3&nbsp;-&nbsp;Q1</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Define&nbsp;bounds&nbsp;for&nbsp;outliers</span></span><br><span><span class="mtk1">lower_bound&nbsp;=&nbsp;Q1&nbsp;-&nbsp;</span><span class="mtk6">1.5</span><span class="mtk1">&nbsp;*&nbsp;IQR</span></span><br><span><span class="mtk1">upper_bound&nbsp;=&nbsp;Q3&nbsp;+&nbsp;</span><span class="mtk6">1.5</span><span class="mtk1">&nbsp;*&nbsp;IQR</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Cap&nbsp;outliers&nbsp;in&nbsp;duration_sec</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'duration_sec'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'duration_sec'</span><span class="mtk12">]</span><span class="mtk1">.clip</span><span class="mtk12">(</span><span class="mtk1">lower=lower_bound</span><span class="mtk12">,</span><span class="mtk1">&nbsp;upper=upper_bound</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk1">display</span><span class="mtk12">(</span><span class="mtk1">df.head</span><span class="mtk12">())</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$050605479$-->Start coding or <span role="button" class="link" tabindex="0">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 9 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div class="outputview" style="height: 851px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals" src="./Untitled21.ipynb - Colab_files/outputframe(2).html" class="" style="height: 851px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell text" id="cell-LtKX5ecKkkkG" role="region" aria-label="Cell 10: Text cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><p><strong>Reasoning</strong>:
Fix the previous code block to address the <code>FutureWarning</code> about chained assignment and display the updated DataFrame.</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>0 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code icon-scrolling code-has-output" id="cell-V_lEAnZ8kkz2" role="region" aria-label="Cell 11: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
12:55 AM (28 minutes ago)
executed in 0.172s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->12:55 AM (28 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 0.172s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab-dark colab-dark colab-dark colab-dark colab-dark" data-lang="notebook-python"><span><span class="mtk8">#&nbsp;Fill&nbsp;missing&nbsp;station&nbsp;names&nbsp;with&nbsp;'Unknown'</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'start_station_name'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'start_station_name'</span><span class="mtk12">]</span><span class="mtk1">.fillna</span><span class="mtk12">(</span><span class="mtk5">'Unknown'</span><span class="mtk12">)</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'end_station_name'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'end_station_name'</span><span class="mtk12">]</span><span class="mtk1">.fillna</span><span class="mtk12">(</span><span class="mtk5">'Unknown'</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Fill&nbsp;missing&nbsp;gender&nbsp;with&nbsp;the&nbsp;mode</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'member_gender'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'member_gender'</span><span class="mtk12">]</span><span class="mtk1">.fillna</span><span class="mtk12">(</span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'member_gender'</span><span class="mtk12">]</span><span class="mtk1">.mode</span><span class="mtk12">()[</span><span class="mtk6">0</span><span class="mtk12">])</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Impute&nbsp;missing&nbsp;birth&nbsp;years&nbsp;with&nbsp;the&nbsp;median</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'member_birth_year'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'member_birth_year'</span><span class="mtk12">]</span><span class="mtk1">.fillna</span><span class="mtk12">(</span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'member_birth_year'</span><span class="mtk12">]</span><span class="mtk1">.median</span><span class="mtk12">())</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Calculate&nbsp;the&nbsp;IQR&nbsp;for&nbsp;duration_sec</span></span><br><span><span class="mtk1">Q1&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'duration_sec'</span><span class="mtk12">]</span><span class="mtk1">.quantile</span><span class="mtk12">(</span><span class="mtk6">0.25</span><span class="mtk12">)</span></span><br><span><span class="mtk1">Q3&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'duration_sec'</span><span class="mtk12">]</span><span class="mtk1">.quantile</span><span class="mtk12">(</span><span class="mtk6">0.75</span><span class="mtk12">)</span></span><br><span><span class="mtk1">IQR&nbsp;=&nbsp;Q3&nbsp;-&nbsp;Q1</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Define&nbsp;bounds&nbsp;for&nbsp;outliers</span></span><br><span><span class="mtk1">lower_bound&nbsp;=&nbsp;Q1&nbsp;-&nbsp;</span><span class="mtk6">1.5</span><span class="mtk1">&nbsp;*&nbsp;IQR</span></span><br><span><span class="mtk1">upper_bound&nbsp;=&nbsp;Q3&nbsp;+&nbsp;</span><span class="mtk6">1.5</span><span class="mtk1">&nbsp;*&nbsp;IQR</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Cap&nbsp;outliers&nbsp;in&nbsp;duration_sec</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'duration_sec'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'duration_sec'</span><span class="mtk12">]</span><span class="mtk1">.clip</span><span class="mtk12">(</span><span class="mtk1">lower=lower_bound</span><span class="mtk12">,</span><span class="mtk1">&nbsp;upper=upper_bound</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk1">display</span><span class="mtk12">(</span><span class="mtk1">df.head</span><span class="mtk12">())</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$050605479$-->Start coding or <span role="button" class="link" tabindex="0">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 11 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div class="outputview" style="height: 365px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals" src="./Untitled21.ipynb - Colab_files/outputframe(3).html" class="" style="height: 365px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell text" id="cell-D6FKxcwZkoGF" role="region" aria-label="Cell 12: Text cell: Data wrangling" style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><div class="text-cell-section-header layout horizontal center"><md-icon-button class="header-section-toggle" title="Collapse 2 child cells under Data wrangling (Press &lt;Shift&gt; to also collapse sibling sections)" data-aria-label="Collapse 2 child cells under Data wrangling (Press &lt;Shift&gt; to also collapse sibling sections)" style="" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Collapse 2 child cells under Data wrangling (Press &lt;Shift&gt; to also collapse sibling sections)">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>keyboard_arrow_down</md-icon></md-icon-button><h2>Data wrangling</h2></div>
<h3>Subtask:</h3>
<p>Create new features and transform existing ones to prepare the data for analysis.</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class=" cell-execution ">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>2 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell text" id="cell-NLgSFuK1ko9T" role="region" aria-label="Cell 13: Text cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><p><strong>Reasoning</strong>:
Create new features as requested in the instructions, including trip duration in minutes, day of the week, user age, and age groups.</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>0 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code icon-scrolling code-has-output" id="cell-CB3gBPHokpNF" role="region" aria-label="Cell 14: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
12:56 AM (28 minutes ago)
executed in 0.247s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->12:56 AM (28 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 0.247s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab-dark colab-dark colab-dark colab-dark colab-dark" data-lang="notebook-python"><span><span class="mtk18">import</span><span class="mtk1">&nbsp;pandas&nbsp;</span><span class="mtk18">as</span><span class="mtk1">&nbsp;pd</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;1.&nbsp;Trip&nbsp;Duration&nbsp;in&nbsp;Minutes</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'duration_min'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'duration_sec'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;/&nbsp;</span><span class="mtk6">60</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;2.&nbsp;Day&nbsp;of&nbsp;the&nbsp;Week</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'start_time'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;pd.to_datetime</span><span class="mtk12">(</span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'start_time'</span><span class="mtk12">])</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'day_of_week'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'start_time'</span><span class="mtk12">]</span><span class="mtk1">.dt.day_name</span><span class="mtk12">()</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;3.&nbsp;User&nbsp;Age</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'user_age'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;</span><span class="mtk6">2019</span><span class="mtk1">&nbsp;-&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'member_birth_year'</span><span class="mtk12">]</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Handle&nbsp;potential&nbsp;errors&nbsp;in&nbsp;user&nbsp;age&nbsp;(replace&nbsp;unr</span><span class="mtk8">easonable&nbsp;ages)</span></span><br><span><span class="mtk1">df.loc</span><span class="mtk12">[(</span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'user_age'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;&lt;&nbsp;</span><span class="mtk6">0</span><span class="mtk12">)</span><span class="mtk1">&nbsp;|&nbsp;</span><span class="mtk12">(</span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'user_age'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;&gt;&nbsp;</span><span class="mtk6">100</span><span class="mtk12">),</span><span class="mtk1">&nbsp;</span><span class="mtk5">'user_age'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;</span><span class="mtk9">None</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;4.&nbsp;Age&nbsp;Groups</span></span><br><span><span class="mtk9">def</span><span class="mtk1">&nbsp;</span><span class="mtk15">categorize_age</span><span class="mtk1">(</span><span class="mtk4">age</span><span class="mtk1">)</span><span class="mtk12">:</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk18">if</span><span class="mtk1">&nbsp;</span><span class="mtk6">0</span><span class="mtk1">&nbsp;&lt;=&nbsp;age&nbsp;&lt;=&nbsp;</span><span class="mtk6">17</span><span class="mtk12">:</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk18">return</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Youth'</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk18">elif</span><span class="mtk1">&nbsp;</span><span class="mtk6">18</span><span class="mtk1">&nbsp;&lt;=&nbsp;age&nbsp;&lt;=&nbsp;</span><span class="mtk6">34</span><span class="mtk12">:</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk18">return</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Young&nbsp;Adult'</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk18">elif</span><span class="mtk1">&nbsp;</span><span class="mtk6">35</span><span class="mtk1">&nbsp;&lt;=&nbsp;age&nbsp;&lt;=&nbsp;</span><span class="mtk6">64</span><span class="mtk12">:</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk18">return</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Adult'</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk18">elif</span><span class="mtk1">&nbsp;age&nbsp;&gt;=&nbsp;</span><span class="mtk6">65</span><span class="mtk12">:</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk18">return</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Senior'</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk18">else</span><span class="mtk12">:</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk18">return</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Unknown'</span><span class="mtk1">&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Handle&nbsp;missing&nbsp;or&nbsp;invalid&nbsp;ages</span></span><br><span><span></span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'age_group'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'user_age'</span><span class="mtk12">]</span><span class="mtk1">.apply</span><span class="mtk12">(</span><span class="mtk1">categorize_age</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk1">display</span><span class="mtk12">(</span><span class="mtk1">df.head</span><span class="mtk12">())</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$050605479$-->Start coding or <span role="button" class="link" tabindex="0">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 14 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div class="outputview" style="height: 394px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals" src="./Untitled21.ipynb - Colab_files/outputframe(4).html" class="" style="height: 394px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell text" id="cell-kMsmlYZxktLO" role="region" aria-label="Cell 15: Text cell: Data analysis" style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><div class="text-cell-section-header layout horizontal center"><md-icon-button class="header-section-toggle" title="Collapse 2 child cells under Data analysis (Press &lt;Shift&gt; to also collapse sibling sections)" data-aria-label="Collapse 2 child cells under Data analysis (Press &lt;Shift&gt; to also collapse sibling sections)" style="" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Collapse 2 child cells under Data analysis (Press &lt;Shift&gt; to also collapse sibling sections)">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>keyboard_arrow_down</md-icon></md-icon-button><h2>Data analysis</h2></div>
<h3>Subtask:</h3>
<p>Analyze the prepared data to identify trends and patterns.</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>2 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell text" id="cell-k_NvFx6hkuBB" role="region" aria-label="Cell 16: Text cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><p><strong>Reasoning</strong>:
Calculate descriptive statistics for <code>duration_min</code> grouped by <code>user_type</code> and <code>day_of_week</code>, determine popular start/end stations, analyze user age distribution, and investigate correlations between variables.</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>0 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling code-has-output" id="cell-O86g1zRSkuQz" role="region" aria-label="Cell 17: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
12:56 AM (27 minutes ago)
executed in 0.428s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->12:56 AM (27 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 0.428s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark" data-lang="notebook-python"><span><span class="mtk8">#&nbsp;1.&nbsp;Descriptive&nbsp;statistics&nbsp;for&nbsp;duration_min</span></span><br><span><span class="mtk1">duration_stats&nbsp;=&nbsp;df.groupby</span><span class="mtk12">([</span><span class="mtk5">'user_type'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'day_of_week'</span><span class="mtk12">])[</span><span class="mtk5">'duration_min'</span><span class="mtk12">]</span><span class="mtk1">.agg</span><span class="mtk12">([</span><span class="mtk5">'mean'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'median'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'std'</span><span class="mtk12">])</span></span><br><span><span class="mtk1">display</span><span class="mtk12">(</span><span class="mtk1">duration_stats</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;2.&nbsp;Popular&nbsp;start&nbsp;and&nbsp;end&nbsp;stations</span></span><br><span><span class="mtk1">popular_start_stations&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'start_station_name'</span><span class="mtk12">]</span><span class="mtk1">.value_counts</span><span class="mtk12">()</span><span class="mtk1">.head</span><span class="mtk12">(</span><span class="mtk6">10</span><span class="mtk12">)</span></span><br><span><span class="mtk1">popular_end_stations&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'end_station_name'</span><span class="mtk12">]</span><span class="mtk1">.value_counts</span><span class="mtk12">()</span><span class="mtk1">.head</span><span class="mtk12">(</span><span class="mtk6">10</span><span class="mtk12">)</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"Popular&nbsp;Start&nbsp;Stations:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;popular_start_stations</span><span class="mtk12">)</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"\nPopular&nbsp;End&nbsp;Stations:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;popular_end_stations</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Analyze&nbsp;popular&nbsp;stations&nbsp;by&nbsp;user&nbsp;type&nbsp;and&nbsp;day&nbsp;of</span><span class="mtk8">&nbsp;week&nbsp;(example&nbsp;for&nbsp;start&nbsp;stations)</span></span><br><span><span class="mtk1">start_station_by_usertype&nbsp;=&nbsp;df.groupby</span><span class="mtk12">([</span><span class="mtk5">'user_type'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'day_of_week'</span><span class="mtk12">])[</span><span class="mtk5">'start_station_name'</span><span class="mtk12">]</span><span class="mtk1">.value_counts</span><span class="mtk12">()</span><span class="mtk1">.unstack</span><span class="mtk12">()</span></span><br><span><span class="mtk8">#&nbsp;Displaying&nbsp;the&nbsp;first&nbsp;few&nbsp;to&nbsp;avoid&nbsp;large&nbsp;output.</span></span><br><span><span class="mtk1">display</span><span class="mtk12">(</span><span class="mtk1">start_station_by_usertype.head</span><span class="mtk12">(</span><span class="mtk6">10</span><span class="mtk12">))</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;3.&nbsp;User&nbsp;age&nbsp;distribution</span></span><br><span><span class="mtk1">age_distribution&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'user_age'</span><span class="mtk12">]</span><span class="mtk1">.describe</span><span class="mtk12">()</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"\nUser&nbsp;Age&nbsp;Distribution:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;age_distribution</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk1">unknown_age_characteristics&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'age_group'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;==&nbsp;</span><span class="mtk5">'Unknown'</span><span class="mtk12">]</span><span class="mtk1">.describe</span><span class="mtk12">()</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"\nCharacteristics&nbsp;of&nbsp;Unknown&nbsp;Age&nbsp;Group:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;unknown_age_characteristics</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;4.&nbsp;Correlation&nbsp;analysis</span></span><br><span><span class="mtk1">correlation_matrix&nbsp;=&nbsp;df</span><span class="mtk12">[[</span><span class="mtk5">'duration_min'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'user_age'</span><span class="mtk12">]]</span><span class="mtk1">.corr</span><span class="mtk12">()</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"\nCorrelation&nbsp;Matrix:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;correlation_matrix</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Additional&nbsp;correlation&nbsp;analysis&nbsp;(example&nbsp;with&nbsp;us</span><span class="mtk8">er_type)</span></span><br><span><span class="mtk8">#&nbsp;Note:&nbsp;user_type&nbsp;is&nbsp;categorical,&nbsp;so&nbsp;we&nbsp;need&nbsp;to&nbsp;co</span><span class="mtk8">nvert&nbsp;it&nbsp;to&nbsp;numerical&nbsp;for&nbsp;correlation</span></span><br><span><span class="mtk8">#&nbsp;This&nbsp;is&nbsp;a&nbsp;simple&nbsp;way&nbsp;for&nbsp;demonstrating&nbsp;purposes&nbsp;</span><span class="mtk8">only.&nbsp;&nbsp;More&nbsp;robust&nbsp;methods&nbsp;may&nbsp;be&nbsp;needed</span></span><br><span><span class="mtk1">user_type_mapping&nbsp;=&nbsp;</span><span class="mtk12">{</span><span class="mtk5">'Subscriber'</span><span class="mtk12">:</span><span class="mtk1">&nbsp;</span><span class="mtk6">1</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Customer'</span><span class="mtk12">:</span><span class="mtk1">&nbsp;</span><span class="mtk6">0</span><span class="mtk12">}</span></span><br><span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'user_type_numeric'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'user_type'</span><span class="mtk12">]</span><span class="mtk1">.</span><span class="mtk15">map</span><span class="mtk12">(</span><span class="mtk1">user_type_mapping</span><span class="mtk12">)</span></span><br><span><span class="mtk1">correlation_matrix_with_usertype&nbsp;=&nbsp;df</span><span class="mtk12">[[</span><span class="mtk5">'duration_min'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'user_type_numeric'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'user_age'</span><span class="mtk12">]]</span><span class="mtk1">.corr</span><span class="mtk12">()</span></span><br><span><span class="mtk15">print</span><span class="mtk12">(</span><span class="mtk5">"\nCorrelation&nbsp;Matrix&nbsp;including&nbsp;user_type:\n"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;correlation_matrix_with_usertype</span><span class="mtk12">)</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$050605479$-->Start coding or <span role="button" class="link" tabindex="0">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 17 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div class="outputview" style="height: 1000px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals" src="./Untitled21.ipynb - Colab_files/outputframe(5).html" class="" style="height: 1000px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps hascontent=""><template shadowrootmode="open"><!----> <div class="root">
        <span class="next-steps-title">
          <!--?lit$050605479$-->Next steps: </span><!--?lit$050605479$--><!----><md-outlined-button value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
            <!--?lit$050605479$-->Generate code with <code>duration_stats</code>
          </md-outlined-button><!----><!----><md-outlined-button class="plots" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
            <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>
              <!--?lit$050605479$-->toggle_off
            </md-icon>
            <!--?lit$050605479$-->View recommended plots
          </md-outlined-button><!----><!----><md-outlined-button class="interactive-sheet" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
            New interactive sheet
          </md-outlined-button><!---->
      </div>
      <div class="content"><!--?lit$050605479$--></div></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell text" id="cell-gyhDX9LckxnI" role="region" aria-label="Cell 18: Text cell: Data visualization" style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><div class="text-cell-section-header layout horizontal center"><md-icon-button class="header-section-toggle" title="Collapse 2 child cells under Data visualization (Press &lt;Shift&gt; to also collapse sibling sections)" data-aria-label="Collapse 2 child cells under Data visualization (Press &lt;Shift&gt; to also collapse sibling sections)" style="" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Collapse 2 child cells under Data visualization (Press &lt;Shift&gt; to also collapse sibling sections)">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>keyboard_arrow_down</md-icon></md-icon-button><h2>Data visualization</h2></div>
<h3>Subtask:</h3>
<p>Visualize the key findings from the data analysis.</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>2 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell text" id="cell-6V-46vEtkzHc" role="region" aria-label="Cell 19: Text cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><p><strong>Reasoning</strong>:
Generate the visualizations specified in the instructions using the prepared dataframe.</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class=" cell-execution ">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>0 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code icon-scrolling code-has-output" id="cell-w_Ps88TckzXX" role="region" aria-label="Cell 20: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
12:56 AM (27 minutes ago)
executed in 6.657s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->12:56 AM (27 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 6.657s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><div class="editor flex monaco" data-keybinding-context="142" data-mode-id="notebook-python" style="height: 1074px; --vscode-editorCodeLens-lineHeight: 16px; --vscode-editorCodeLens-fontSize: 12px; --vscode-editorCodeLens-fontFeatureSettings: &quot;liga&quot; off, &quot;calt&quot; off;"><div class="monaco-editor no-user-select  showUnused showDeprecated vs-dark" role="code" data-uri="inmemory://model/24" style="width: 1192px; height: 1074px;"><div data-mprt="3" class="overflow-guard" style="width: 1192px; height: 1074px; overflow: clip;"><div class="margin" role="presentation" aria-hidden="true" style="position: absolute; contain: strict; will-change: unset; top: 0px; height: 1074px; width: 6px;"><div class="glyph-margin" style="left: 0px; width: 0px; height: 1074px;"></div><div class="margin-view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="margin-view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 6px; height: 1074px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line current-line-margin-both" style="width:6px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div><div style="position:absolute;top:323px;width:100%;height:19px;"></div><div style="position:absolute;top:342px;width:100%;height:19px;"></div><div style="position:absolute;top:361px;width:100%;height:19px;"></div><div style="position:absolute;top:380px;width:100%;height:19px;"></div><div style="position:absolute;top:399px;width:100%;height:19px;"></div><div style="position:absolute;top:418px;width:100%;height:19px;"></div><div style="position:absolute;top:437px;width:100%;height:19px;"></div><div style="position:absolute;top:456px;width:100%;height:19px;"></div><div style="position:absolute;top:475px;width:100%;height:19px;"></div><div style="position:absolute;top:494px;width:100%;height:19px;"></div><div style="position:absolute;top:513px;width:100%;height:19px;"></div><div style="position:absolute;top:532px;width:100%;height:19px;"></div><div style="position:absolute;top:551px;width:100%;height:19px;"></div><div style="position:absolute;top:570px;width:100%;height:19px;"></div><div style="position:absolute;top:589px;width:100%;height:19px;"></div><div style="position:absolute;top:608px;width:100%;height:19px;"></div><div style="position:absolute;top:627px;width:100%;height:19px;"></div><div style="position:absolute;top:646px;width:100%;height:19px;"></div><div style="position:absolute;top:665px;width:100%;height:19px;"></div><div style="position:absolute;top:684px;width:100%;height:19px;"></div><div style="position:absolute;top:703px;width:100%;height:19px;"></div><div style="position:absolute;top:722px;width:100%;height:19px;"></div><div style="position:absolute;top:741px;width:100%;height:19px;"></div><div style="position:absolute;top:760px;width:100%;height:19px;"></div><div style="position:absolute;top:779px;width:100%;height:19px;"></div><div style="position:absolute;top:798px;width:100%;height:19px;"></div><div style="position:absolute;top:817px;width:100%;height:19px;"></div><div style="position:absolute;top:836px;width:100%;height:19px;"></div><div style="position:absolute;top:855px;width:100%;height:19px;"></div><div style="position:absolute;top:874px;width:100%;height:19px;"></div><div style="position:absolute;top:893px;width:100%;height:19px;"></div><div style="position:absolute;top:912px;width:100%;height:19px;"></div><div style="position:absolute;top:931px;width:100%;height:19px;"></div><div style="position:absolute;top:950px;width:100%;height:19px;"></div><div style="position:absolute;top:969px;width:100%;height:19px;"></div><div style="position:absolute;top:988px;width:100%;height:19px;"></div><div style="position:absolute;top:1007px;width:100%;height:19px;"></div><div style="position:absolute;top:1026px;width:100%;height:19px;"></div><div style="position:absolute;top:1045px;width:100%;height:19px;"></div></div><div class="glyph-margin-widgets" style="position: absolute; top: 0px;"></div></div><div class="monaco-scrollable-element editor-scrollable vs-dark" role="presentation" data-mprt="5" style="position: absolute; overflow: hidden; left: 6px; width: 1186px; height: 1074px;"><div class="lines-content monaco-editor-background" style="position: absolute; overflow: hidden; width: 1e+06px; height: 1074px; contain: strict; will-change: unset; top: 0px; left: 0px;"><div class="view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; height: 0px; width: 1207px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line" style="width:1207px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div><div style="position:absolute;top:323px;width:100%;height:19px;"></div><div style="position:absolute;top:342px;width:100%;height:19px;"></div><div style="position:absolute;top:361px;width:100%;height:19px;"></div><div style="position:absolute;top:380px;width:100%;height:19px;"></div><div style="position:absolute;top:399px;width:100%;height:19px;"></div><div style="position:absolute;top:418px;width:100%;height:19px;"></div><div style="position:absolute;top:437px;width:100%;height:19px;"></div><div style="position:absolute;top:456px;width:100%;height:19px;"></div><div style="position:absolute;top:475px;width:100%;height:19px;"></div><div style="position:absolute;top:494px;width:100%;height:19px;"></div><div style="position:absolute;top:513px;width:100%;height:19px;"></div><div style="position:absolute;top:532px;width:100%;height:19px;"></div><div style="position:absolute;top:551px;width:100%;height:19px;"></div><div style="position:absolute;top:570px;width:100%;height:19px;"></div><div style="position:absolute;top:589px;width:100%;height:19px;"></div><div style="position:absolute;top:608px;width:100%;height:19px;"></div><div style="position:absolute;top:627px;width:100%;height:19px;"></div><div style="position:absolute;top:646px;width:100%;height:19px;"></div><div style="position:absolute;top:665px;width:100%;height:19px;"></div><div style="position:absolute;top:684px;width:100%;height:19px;"></div><div style="position:absolute;top:703px;width:100%;height:19px;"></div><div style="position:absolute;top:722px;width:100%;height:19px;"></div><div style="position:absolute;top:741px;width:100%;height:19px;"></div><div style="position:absolute;top:760px;width:100%;height:19px;"></div><div style="position:absolute;top:779px;width:100%;height:19px;"></div><div style="position:absolute;top:798px;width:100%;height:19px;"></div><div style="position:absolute;top:817px;width:100%;height:19px;"></div><div style="position:absolute;top:836px;width:100%;height:19px;"></div><div style="position:absolute;top:855px;width:100%;height:19px;"></div><div style="position:absolute;top:874px;width:100%;height:19px;"></div><div style="position:absolute;top:893px;width:100%;height:19px;"></div><div style="position:absolute;top:912px;width:100%;height:19px;"></div><div style="position:absolute;top:931px;width:100%;height:19px;"></div><div style="position:absolute;top:950px;width:100%;height:19px;"></div><div style="position:absolute;top:969px;width:100%;height:19px;"></div><div style="position:absolute;top:988px;width:100%;height:19px;"></div><div style="position:absolute;top:1007px;width:100%;height:19px;"></div><div style="position:absolute;top:1026px;width:100%;height:19px;"></div><div style="position:absolute;top:1045px;width:100%;height:19px;"></div></div><div role="presentation" aria-hidden="true" class="view-rulers"><div class="view-ruler" style="width: 2px; height: 1074px; left: 615.938px;"></div></div><div class="view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="view-lines monaco-mouse-cursor-text" role="presentation" aria-hidden="true" data-mprt="7" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 1207px; height: 1074px;"><div style="top:0px;height:19px;" class="view-line"><span><span class="mtk18">import</span><span class="mtk1">&nbsp;matplotlib.pyplot&nbsp;</span><span class="mtk18">as</span><span class="mtk1">&nbsp;plt</span></span></div><div style="top:19px;height:19px;" class="view-line"><span><span class="mtk18">import</span><span class="mtk1">&nbsp;seaborn&nbsp;</span><span class="mtk18">as</span><span class="mtk1">&nbsp;sns</span></span></div><div style="top:38px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:57px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;1.&nbsp;Trip&nbsp;Duration&nbsp;Distribution</span></span></div><div style="top:76px;height:19px;" class="view-line"><span><span class="mtk1">plt.figure</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">figsize=</span><span class="mtk12 bracket-highlighting-1">(</span><span class="mtk6">10</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk6">6</span><span class="mtk12 bracket-highlighting-1">)</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:95px;height:19px;" class="view-line"><span><span class="mtk1">sns.boxplot</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">x=</span><span class="mtk5">'user_type'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;y=</span><span class="mtk5">'duration_min'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;data=df</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:114px;height:19px;" class="view-line"><span><span class="mtk1">plt.title</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'Trip&nbsp;Duration&nbsp;Distribution&nbsp;by&nbsp;User&nbsp;Type'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:133px;height:19px;" class="view-line"><span><span class="mtk1">plt.xlabel</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'User&nbsp;Type'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:152px;height:19px;" class="view-line"><span><span class="mtk1">plt.ylabel</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'Trip&nbsp;Duration&nbsp;(minutes)'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:171px;height:19px;" class="view-line"><span><span class="mtk1">plt.show</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:190px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:209px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;2.&nbsp;Daily&nbsp;Trip&nbsp;Patterns</span></span></div><div style="top:228px;height:19px;" class="view-line"><span><span class="mtk1">trips_per_day&nbsp;=&nbsp;df.groupby</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'day_of_week'</span><span class="mtk12 bracket-highlighting-0">)</span><span class="mtk12 bracket-highlighting-0">[</span><span class="mtk5">'start_time'</span><span class="mtk12 bracket-highlighting-0">]</span><span class="mtk1">.count</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span><span class="mtk1">.reindex</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-1">[</span><span class="mtk5">'Monday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Tuesday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Wednesday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Thursday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Friday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Saturday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Sunday'</span><span class="mtk12 bracket-highlighting-1">]</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:247px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:266px;height:19px;" class="view-line"><span><span class="mtk1">plt.figure</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">figsize=</span><span class="mtk12 bracket-highlighting-1">(</span><span class="mtk6">10</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk6">6</span><span class="mtk12 bracket-highlighting-1">)</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:285px;height:19px;" class="view-line"><span><span class="mtk1">plt.plot</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">trips_per_day.index</span><span class="mtk12">,</span><span class="mtk1">&nbsp;trips_per_day.values</span><span class="mtk12">,</span><span class="mtk1">&nbsp;marker=</span><span class="mtk5">'o'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;linestyle=</span><span class="mtk5">'-'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;color=</span><span class="mtk5">'skyblue'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:304px;height:19px;" class="view-line"><span><span class="mtk1">plt.title</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'Daily&nbsp;Trip&nbsp;Patterns'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:323px;height:19px;" class="view-line"><span><span class="mtk1">plt.xlabel</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'Day&nbsp;of&nbsp;the&nbsp;Week'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:342px;height:19px;" class="view-line"><span><span class="mtk1">plt.ylabel</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'Number&nbsp;of&nbsp;Trips'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:361px;height:19px;" class="view-line"><span><span class="mtk1">plt.xticks</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">rotation=</span><span class="mtk6">45</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:380px;height:19px;" class="view-line"><span><span class="mtk1">plt.tight_layout</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:399px;height:19px;" class="view-line"><span><span class="mtk1">plt.show</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:418px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:437px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:456px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;3.&nbsp;Popular&nbsp;Start&nbsp;Stations</span></span></div><div style="top:475px;height:19px;" class="view-line"><span><span class="mtk1">plt.figure</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">figsize=</span><span class="mtk12 bracket-highlighting-1">(</span><span class="mtk6">10</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk6">6</span><span class="mtk12 bracket-highlighting-1">)</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:494px;height:19px;" class="view-line"><span><span class="mtk1">popular_start_stations&nbsp;=&nbsp;df</span><span class="mtk12 bracket-highlighting-0">[</span><span class="mtk5">'start_station_name'</span><span class="mtk12 bracket-highlighting-0">]</span><span class="mtk1">.value_counts</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span><span class="mtk1">.head</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk6">10</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:513px;height:19px;" class="view-line"><span><span class="mtk1">plt.barh</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">popular_start_stations.index</span><span class="mtk12">,</span><span class="mtk1">&nbsp;popular_start_stations.values</span><span class="mtk12">,</span><span class="mtk1">&nbsp;color=</span><span class="mtk5">'lightcoral'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:532px;height:19px;" class="view-line"><span><span class="mtk1">plt.title</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'Top&nbsp;10&nbsp;Most&nbsp;Popular&nbsp;Start&nbsp;Stations'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:551px;height:19px;" class="view-line"><span><span class="mtk1">plt.xlabel</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'Number&nbsp;of&nbsp;Trips'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:570px;height:19px;" class="view-line"><span><span class="mtk1">plt.ylabel</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'Start&nbsp;Station&nbsp;Name'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:589px;height:19px;" class="view-line"><span><span class="mtk1">plt.gca</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span><span class="mtk1">.invert_yaxis</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span><span class="mtk1">&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Invert&nbsp;y-axis&nbsp;to&nbsp;show&nbsp;most&nbsp;popular&nbsp;at&nbsp;the&nbsp;top</span></span></div><div style="top:608px;height:19px;" class="view-line"><span><span class="mtk1">plt.tight_layout</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:627px;height:19px;" class="view-line"><span><span class="mtk1">plt.show</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:646px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:665px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;4.&nbsp;User&nbsp;Age&nbsp;Distribution</span></span></div><div style="top:684px;height:19px;" class="view-line"><span><span class="mtk1">plt.figure</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">figsize=</span><span class="mtk12 bracket-highlighting-1">(</span><span class="mtk6">12</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk6">5</span><span class="mtk12 bracket-highlighting-1">)</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:703px;height:19px;" class="view-line"><span><span class="mtk1">plt.subplot</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk6">1</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk6">2</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk6">1</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:722px;height:19px;" class="view-line"><span><span class="mtk1">plt.hist</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">df</span><span class="mtk12 bracket-highlighting-1">[</span><span class="mtk5">'user_age'</span><span class="mtk12 bracket-highlighting-1">]</span><span class="mtk1">.dropna</span><span class="mtk12 bracket-highlighting-1">(</span><span class="mtk12 bracket-highlighting-1">)</span><span class="mtk12">,</span><span class="mtk1">&nbsp;bins=</span><span class="mtk6">20</span><span class="mtk12">,</span><span class="mtk1">&nbsp;color=</span><span class="mtk5">'lightgreen'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;edgecolor=</span><span class="mtk5">'black'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:741px;height:19px;" class="view-line"><span><span class="mtk1">plt.title</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'User&nbsp;Age&nbsp;Distribution'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:760px;height:19px;" class="view-line"><span><span class="mtk1">plt.xlabel</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'User&nbsp;Age'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:779px;height:19px;" class="view-line"><span><span class="mtk1">plt.ylabel</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'Frequency'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:798px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:817px;height:19px;" class="view-line"><span><span class="mtk1">plt.subplot</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk6">1</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk6">2</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk6">2</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:836px;height:19px;" class="view-line"><span><span class="mtk1">sns.boxplot</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">x=</span><span class="mtk5">'user_type'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;y=</span><span class="mtk5">'user_age'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;data=df</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:855px;height:19px;" class="view-line"><span><span class="mtk1">plt.title</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'User&nbsp;Age&nbsp;Distribution&nbsp;by&nbsp;User&nbsp;Type'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:874px;height:19px;" class="view-line"><span><span class="mtk1">plt.xlabel</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'User&nbsp;Type'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:893px;height:19px;" class="view-line"><span><span class="mtk1">plt.ylabel</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'User&nbsp;Age'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:912px;height:19px;" class="view-line"><span><span class="mtk1">plt.tight_layout</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:931px;height:19px;" class="view-line"><span><span class="mtk1">plt.show</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:950px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:969px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;5.&nbsp;Correlation&nbsp;Visualization&nbsp;(Optional)</span></span></div><div style="top:988px;height:19px;" class="view-line"><span><span class="mtk1">plt.figure</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">figsize=</span><span class="mtk12 bracket-highlighting-1">(</span><span class="mtk6">8</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk6">6</span><span class="mtk12 bracket-highlighting-1">)</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:1007px;height:19px;" class="view-line"><span><span class="mtk1">sns.heatmap</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">correlation_matrix_with_usertype</span><span class="mtk12">,</span><span class="mtk1">&nbsp;annot=</span><span class="mtk9">True</span><span class="mtk12">,</span><span class="mtk1">&nbsp;cmap=</span><span class="mtk5">'viridis'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;fmt=</span><span class="mtk5">".2f"</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:1026px;height:19px;" class="view-line"><span><span class="mtk1">plt.title</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk5">'Correlation&nbsp;Matrix'</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:1045px;height:19px;" class="view-line"><span><span class="mtk1">plt.show</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span></span></div></div><div data-mprt="1" class="contentWidgets" style="position: absolute; top: 0px;"></div><div role="presentation" aria-hidden="true" class="cursors-layer cursor-line-style cursor-solid"><div class="cursor monaco-mouse-cursor-text " style="height: 19px; top: 0px; left: 0px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; display: block; visibility: hidden; padding-left: 0px; width: 1.6px;"></div></div></div><div role="presentation" aria-hidden="true" class="visible scrollbar horizontal" style="position: absolute; width: 1172px; height: 10px; left: 0px; bottom: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; width: 1151px;"></div></div><canvas class="decorationsOverviewRuler" aria-hidden="true" width="17" height="1342" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; top: 0px; right: 0px; width: 14px; height: 1074px; will-change: unset; display: block;"></canvas><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute; width: 14px; height: 1074px; right: 0px; top: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 14px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; height: 1074px;"></div></div></div><div role="presentation" aria-hidden="true" style="width: 1192px;"></div><textarea data-mprt="6" class="inputarea monaco-mouse-cursor-text" wrap="on" autocorrect="off" autocapitalize="off" autocomplete="off" spellcheck="false" aria-label="Editor content;Press Alt+F1 for Accessibility Options." tabindex="0" role="textbox" aria-roledescription="editor" aria-multiline="true" aria-haspopup="false" aria-autocomplete="both" style="tab-size: 15.3984px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; top: 0px; left: 6px; width: 76992px; height: 1px;"></textarea><div class="monaco-editor-background textAreaCover" style="position: absolute; top: 0px; left: 0px; width: 0px; height: 0px;"></div><div data-mprt="4" class="overlayWidgets" style="width: 1192px;"><div widgetid="editor.contrib.quickInputWidget" style="position: absolute; top: 0px; right: 50%;"></div></div><div data-mprt="8" class="minimap slider-mouseover" role="presentation" aria-hidden="true" style="position: absolute; left: 0px; width: 0px; height: 1074px;"><div class="minimap-shadow-hidden" style="height: 1074px;"></div><canvas width="0" height="1342" style="position: absolute; left: 0px; width: 0px; height: 1074px;"></canvas><canvas class="minimap-decorations-layer" width="0" height="1342" style="position: absolute; left: 0px; width: 0px; height: 1074px;"></canvas><div class="minimap-slider" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; width: 0px; will-change: unset;"><div class="minimap-slider-horizontal" style="position: absolute; width: 0px; height: 0px;"></div></div></div><div role="presentation" aria-hidden="true" class="blockDecorations-container"></div></div><div data-mprt="2" class="overflowingContentWidgets"><div widgetid="editor.contrib.resizableContentHoverWidget" style="position: fixed; height: 10px; width: 10px; z-index: 50; display: none; visibility: hidden; max-width: 1536px;"><div class="monaco-sash vertical" style="left: 8px;"></div><div class="monaco-sash vertical" style="left: -2px;"></div><div class="monaco-sash orthogonal-edge-north horizontal" style="top: -2px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-sash orthogonal-edge-south horizontal" style="top: 8px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-hover hidden" tabindex="0" role="tooltip"><div class="monaco-scrollable-element " role="presentation" style="position: relative; overflow: hidden;"><div class="monaco-hover-content" style="overflow: hidden; font-size: 14px; line-height: 1.35714; max-width: 786.72px; max-height: 268.5px;"></div><div role="presentation" aria-hidden="true" class="invisible scrollbar horizontal" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div class="shadow"></div><div class="shadow"></div><div class="shadow"></div></div></div></div></div><div class=".in-cell-overflowing"></div></div></div></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 20 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div class="outputview" style="height: 1000px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals" src="./Untitled21.ipynb - Colab_files/outputframe(6).html" class="" style="height: 1000px;"></iframe></div></div><div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell text" id="cell-8Rfx2MNzk4ti" role="region" aria-label="Cell 21: Text cell: Summary:" style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><div class="text-cell-section-header layout horizontal center"><md-icon-button class="header-section-toggle" title="Collapse 8 child cells under Summary: (Press &lt;Shift&gt; to also collapse sibling sections)" data-aria-label="Collapse 8 child cells under Summary: (Press &lt;Shift&gt; to also collapse sibling sections)" style="" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Collapse 8 child cells under Summary: (Press &lt;Shift&gt; to also collapse sibling sections)">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>keyboard_arrow_down</md-icon></md-icon-button><h2>Summary:</h2></div>
<h3>1. Q&amp;A</h3>
<p>No questions were explicitly asked in the provided data analysis task. However, the task implicitly asks for insights into the Ford GoBike trip data.  The analysis reveals trends in trip duration, user demographics, and station popularity.</p>
<h3>2. Data Analysis Key Findings</h3>
<ul>
<li><strong>Trip Duration Differences by User Type and Day:</strong> Customers have significantly longer average trip durations than subscribers. Trip durations also vary across the days of the week, with patterns observable for each user type (although the specific patterns weren't detailed).</li>
<li><strong>Popular Stations Vary by User Type and Day:</strong>  While "San Francisco Caltrain Station 2" is a popular end station overall, station popularity varies based on user type (subscriber/customer) and day of the week.</li>
<li><strong>User Age Distribution and Unknown Ages:</strong> The average user age is around 34 years old. A notable portion of users have an "unknown" age group, likely due to missing data.  Further investigation is needed to understand the characteristics of this group.</li>
<li><strong>Weak Correlation Between Trip Duration and Age:</strong> There's a weak positive correlation between trip duration and user age.</li>
<li><strong>Negative Correlation Between Trip Duration and User Type:</strong>  Subscribers tend to have shorter trips than customers, after converting the user type into a numerical representation.  This suggests a difference in usage patterns.</li>
<li><strong>Peak Usage Days:</strong> Weekdays generally show higher numbers of trips compared to weekends, indicating a commute-related usage pattern.</li>
</ul>
<h3>3. Insights or Next Steps</h3>
<ul>
<li><strong>Targeted Marketing:</strong> Analyze the characteristics of the "Unknown" age group.  If a significant portion of potential customers are in this group, consider strategies to collect missing user data.  Use the insights on trip duration and user type to tailor marketing campaigns to specific user segments.</li>
<li><strong>Station Optimization:</strong> Further investigate the variations in station popularity by user type and day of the week to optimize station resources (bike availability, maintenance schedules) and potentially identify opportunities to add new stations.</li>
</ul>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution">
      <button id="run-button" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$-->
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>subdirectory_arrow_right</md-icon>
          <span>8 cells hidden</span>
        </div>
      </div></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling code-has-output" id="cell-IUQtCZ-CmGFm" role="region" aria-label="Cell 22: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
1:03 AM (21 minutes ago)
executed in 39.028s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->1:03 AM (21 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 39.028s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark" data-lang="notebook-python"><span><span class="mtk17">!</span><span class="mtk1">pip&nbsp;install&nbsp;plotly==</span><span class="mtk6">5.15.0</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$050605479$-->Start coding or <span role="button" class="link" tabindex="0">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 22 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div><colab-static-output-renderer role="group" tabindex="0"><div><div class="stream output-id-9 output_text"><pre>Collecting plotly==5.15.0
  Downloading plotly-5.15.0-py2.py3-none-any.whl.metadata (7.0 kB)
Requirement already satisfied: tenacity&gt;=6.2.0 in /usr/local/lib/python3.11/dist-packages (from plotly==5.15.0) (9.0.0)
Requirement already satisfied: packaging in /usr/local/lib/python3.11/dist-packages (from plotly==5.15.0) (24.2)
Downloading plotly-5.15.0-py2.py3-none-any.whl (15.5 MB)
   <span style="color: var(--ansi-bright-black);">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</span><span> </span><span style="color: var(--ansi-green);">15.5/15.5 MB</span><span> </span><span style="color: var(--ansi-red);">17.7 MB/s</span><span> eta </span><span style="color: var(--ansi-cyan);">0:00:00</span><span>
</span>Installing collected packages: plotly
  Attempting uninstall: plotly
    Found existing installation: plotly 5.24.1
    Uninstalling plotly-5.24.1:
      Successfully uninstalled plotly-5.24.1
Successfully installed plotly-5.15.0
</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling" id="cell-3TP51-khmHYp" role="region" aria-label="Cell 23: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
1:03 AM (21 minutes ago)
executed in 0.078s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->1:03 AM (21 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 0.078s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark" data-lang="notebook-python"><span><span class="mtk18">import</span><span class="mtk1">&nbsp;plotly.graph_objects&nbsp;</span><span class="mtk18">as</span><span class="mtk1">&nbsp;go</span></span><br><span><span class="mtk18">from</span><span class="mtk1">&nbsp;plotly.subplots&nbsp;</span><span class="mtk18">import</span><span class="mtk1">&nbsp;make_subplots</span></span><br><span><span class="mtk18">import</span><span class="mtk1">&nbsp;pandas&nbsp;</span><span class="mtk18">as</span><span class="mtk1">&nbsp;pd</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$050605479$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 23 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div><colab-static-output-renderer role="group" tabindex="0"><div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling code-has-output" id="cell-tKPzZyXbmLSL" role="region" aria-label="Cell 24: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
1:03 AM (21 minutes ago)
executed in 4.263s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->1:03 AM (21 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 4.263s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark" data-lang="notebook-python"><span><span class="mtk8">#&nbsp;Trip&nbsp;Duration&nbsp;Distribution&nbsp;by&nbsp;User&nbsp;Type</span></span><br><span><span class="mtk1">fig1&nbsp;=&nbsp;go.Figure</span><span class="mtk12">(</span><span class="mtk1">data=</span><span class="mtk12">[</span><span class="mtk1">go.Box</span><span class="mtk12">(</span><span class="mtk1">y=df</span><span class="mtk12">[</span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'user_type'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;==&nbsp;user_type</span><span class="mtk12">][</span><span class="mtk5">'duration_min'</span><span class="mtk12">],</span><span class="mtk1">&nbsp;name=user_type</span><span class="mtk12">)</span><span class="mtk1">&nbsp;</span><span class="mtk18">for</span><span class="mtk1">&nbsp;user_type&nbsp;</span><span class="mtk17">in</span><span class="mtk1">&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'user_type'</span><span class="mtk12">]</span><span class="mtk1">.unique</span><span class="mtk12">()])</span></span><br><span><span class="mtk1">fig1.update_layout</span><span class="mtk12">(</span><span class="mtk1">title_text=</span><span class="mtk5">"Trip&nbsp;Duration&nbsp;Distribution&nbsp;by&nbsp;User&nbsp;Type"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;yaxis_title=</span><span class="mtk5">"Trip&nbsp;Duration&nbsp;(minutes)"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;xaxis_title=</span><span class="mtk5">"User&nbsp;Type"</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Daily&nbsp;Trip&nbsp;Patterns</span></span><br><span><span class="mtk1">trips_per_day&nbsp;=&nbsp;df.groupby</span><span class="mtk12">(</span><span class="mtk5">'day_of_week'</span><span class="mtk12">)[</span><span class="mtk5">'start_time'</span><span class="mtk12">]</span><span class="mtk1">.count</span><span class="mtk12">()</span><span class="mtk1">.reindex</span><span class="mtk12">([</span><span class="mtk5">'Monday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Tuesday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Wednesday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Thursday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Friday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Saturday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Sunday'</span><span class="mtk12">])</span></span><br><span><span class="mtk1">fig2&nbsp;=&nbsp;go.Figure</span><span class="mtk12">(</span><span class="mtk1">data=</span><span class="mtk12">[</span><span class="mtk1">go.Scatter</span><span class="mtk12">(</span><span class="mtk1">x=trips_per_day.index</span><span class="mtk12">,</span><span class="mtk1">&nbsp;y=trips_per_day.values</span><span class="mtk12">,</span><span class="mtk1">&nbsp;mode=</span><span class="mtk5">'lines+markers'</span><span class="mtk12">)])</span></span><br><span><span class="mtk1">fig2.update_layout</span><span class="mtk12">(</span><span class="mtk1">title_text=</span><span class="mtk5">"Daily&nbsp;Trip&nbsp;Patterns"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;xaxis_title=</span><span class="mtk5">"Day&nbsp;of&nbsp;the&nbsp;Week"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;yaxis_title=</span><span class="mtk5">"Number&nbsp;of&nbsp;Trips"</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Popular&nbsp;Start&nbsp;Stations</span></span><br><span><span class="mtk1">popular_start_stations&nbsp;=&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'start_station_name'</span><span class="mtk12">]</span><span class="mtk1">.value_counts</span><span class="mtk12">()</span><span class="mtk1">.head</span><span class="mtk12">(</span><span class="mtk6">10</span><span class="mtk12">)</span></span><br><span><span class="mtk1">fig3&nbsp;=&nbsp;go.Figure</span><span class="mtk12">(</span><span class="mtk1">data=</span><span class="mtk12">[</span><span class="mtk1">go.Bar</span><span class="mtk12">(</span><span class="mtk1">y=popular_start_stations.index</span><span class="mtk12">,</span><span class="mtk1">&nbsp;x=popular_start_stations.values</span><span class="mtk12">,</span><span class="mtk1">&nbsp;orientation=</span><span class="mtk5">'h'</span><span class="mtk12">)])</span></span><br><span><span class="mtk1">fig3.update_layout</span><span class="mtk12">(</span><span class="mtk1">title_text=</span><span class="mtk5">"Top&nbsp;10&nbsp;Most&nbsp;Popular&nbsp;Start&nbsp;Stations"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;xaxis_title=</span><span class="mtk5">"Number&nbsp;of&nbsp;Trips"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;yaxis_title=</span><span class="mtk5">"Start&nbsp;Station&nbsp;Name"</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;User&nbsp;Age&nbsp;Distribution</span></span><br><span><span class="mtk1">fig4&nbsp;=&nbsp;go.Figure</span><span class="mtk12">(</span><span class="mtk1">data=</span><span class="mtk12">[</span><span class="mtk1">go.Histogram</span><span class="mtk12">(</span><span class="mtk1">x=df</span><span class="mtk12">[</span><span class="mtk5">'user_age'</span><span class="mtk12">]</span><span class="mtk1">.dropna</span><span class="mtk12">())])</span></span><br><span><span class="mtk1">fig4.update_layout</span><span class="mtk12">(</span><span class="mtk1">title_text=</span><span class="mtk5">"User&nbsp;Age&nbsp;Distribution"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;xaxis_title=</span><span class="mtk5">"User&nbsp;Age"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;yaxis_title=</span><span class="mtk5">"Frequency"</span><span class="mtk12">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;User&nbsp;Age&nbsp;Distribution&nbsp;by&nbsp;User&nbsp;Type</span></span><br><span><span class="mtk1">fig5&nbsp;=&nbsp;go.Figure</span><span class="mtk12">(</span><span class="mtk1">data=</span><span class="mtk12">[</span><span class="mtk1">go.Box</span><span class="mtk12">(</span><span class="mtk1">y=df</span><span class="mtk12">[</span><span class="mtk1">df</span><span class="mtk12">[</span><span class="mtk5">'user_type'</span><span class="mtk12">]</span><span class="mtk1">&nbsp;==&nbsp;user_type</span><span class="mtk12">][</span><span class="mtk5">'user_age'</span><span class="mtk12">],</span><span class="mtk1">&nbsp;name=user_type</span><span class="mtk12">)</span><span class="mtk1">&nbsp;</span><span class="mtk18">for</span><span class="mtk1">&nbsp;user_type&nbsp;</span><span class="mtk17">in</span><span class="mtk1">&nbsp;df</span><span class="mtk12">[</span><span class="mtk5">'user_type'</span><span class="mtk12">]</span><span class="mtk1">.unique</span><span class="mtk12">()])</span></span><br><span><span class="mtk1">fig5.update_layout</span><span class="mtk12">(</span><span class="mtk1">title_text=</span><span class="mtk5">"User&nbsp;Age&nbsp;Distribution&nbsp;by&nbsp;User&nbsp;Type"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;yaxis_title=</span><span class="mtk5">"User&nbsp;Age"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;xaxis_title=</span><span class="mtk5">"User&nbsp;Type"</span><span class="mtk12">)</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$050605479$-->Start coding or <span role="button" class="link" tabindex="0">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 24 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div class="outputview" style="height: 542px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals" src="./Untitled21.ipynb - Colab_files/outputframe(7).html" class="" style="height: 542px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling code-has-output focused" id="cell-af5FKJF5mMLV" role="region" aria-label="Cell 25: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"><colab-cell-toolbar><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----> <md-icon-button touch-target="none" aria-describedby="button-move-cell-up-tooltip" data-aria-label="Move cell up
Ctrl+M K" command="move-cell-up" id="button-move-cell-up" value="" style=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Move cell up
Ctrl+M K">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->arrow_upward</md-icon>
        <!--?lit$050605479$-->
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" for="button-move-cell-up" id="button-move-cell-up-tooltip" message="Move cell up
Ctrl+M K"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Move cell up</div><!----><!----><div><!--?lit$050605479$-->Ctrl+M K</div><!----><!--?--></template>
      </colab-tooltip-trigger><!----><!----> <md-icon-button touch-target="none" aria-describedby="button-move-cell-down-tooltip" data-aria-label="Move cell down
Ctrl+M J" command="move-cell-down" id="button-move-cell-down" value="" style=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Move cell down
Ctrl+M J">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->arrow_downward</md-icon>
        <!--?lit$050605479$-->
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" for="button-move-cell-down" id="button-move-cell-down-tooltip" message="Move cell down
Ctrl+M J"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Move cell down</div><!----><!----><div><!--?lit$050605479$-->Ctrl+M J</div><!----><!--?--></template>
      </colab-tooltip-trigger><!----><!----><!--?lit$050605479$--><md-menu positioning="popover" quick="" aria-labelledby="ai-menu-anchor-af5FKJF5mMLV" anchor="ai-menu-anchor-af5FKJF5mMLV" aria-hidden="true"><template shadowrootmode="open"><!---->
      <div class="menu   " popover="manual" style="display: none;">
        <!--?lit$050605479$--><md-elevation part="elevation" aria-hidden="true"><template shadowrootmode="open"><!----><span class="shadow"></span></template></md-elevation>
        <div class="items">
          <div class="item-padding"> <!--?lit$050605479$--><slot></slot> </div>
        </div>
      </div>
    </template>
    <!--?lit$050605479$--><!----><md-menu-item command="generate-code" md-menu-item="" tabindex="0"><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <li id="item" tabindex="0" role="menuitem" class="list-item   "><!--?lit$050605479$-->
      <md-item><template shadowrootmode="open"><!---->
      <slot name="container"></slot>
      <slot class="non-text" name="start"></slot>
      <div class="text">
        <slot name="overline"></slot>
        <slot class="default-slot"></slot>
        <slot name="headline"></slot>
        <slot name="supporting-text"></slot>
      </div>
      <slot class="non-text" name="trailing-supporting-text"></slot>
      <slot class="non-text" name="end"></slot>
    </template>
        <div slot="container">
          <!--?lit$050605479$--> <md-ripple part="ripple" for="item" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple> <!--?lit$050605479$--> <md-focus-ring part="focus-ring" for="item" inward="" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        </div>
        <slot name="start" slot="start"></slot>
        <slot name="end" slot="end"></slot>
        <!--?lit$050605479$-->
      <slot></slot>
      <slot name="overline" slot="overline"></slot>
      <slot name="headline" slot="headline"></slot>
      <slot name="supporting-text" slot="supporting-text"></slot>
      <slot name="trailing-supporting-text" slot="trailing-supporting-text"></slot>
    
      </md-item>
    </li>
    </template>
    <span slot="headline"><!--?lit$050605479$-->Generate code</span>
  </md-menu-item><!----><!----><md-menu-item command="explain-cell" md-menu-item="" tabindex="-1"><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <li id="item" tabindex="0" role="menuitem" class="list-item   "><!--?lit$050605479$-->
      <md-item><template shadowrootmode="open"><!---->
      <slot name="container"></slot>
      <slot class="non-text" name="start"></slot>
      <div class="text">
        <slot name="overline"></slot>
        <slot class="default-slot"></slot>
        <slot name="headline"></slot>
        <slot name="supporting-text"></slot>
      </div>
      <slot class="non-text" name="trailing-supporting-text"></slot>
      <slot class="non-text" name="end"></slot>
    </template>
        <div slot="container">
          <!--?lit$050605479$--> <md-ripple part="ripple" for="item" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple> <!--?lit$050605479$--> <md-focus-ring part="focus-ring" for="item" inward="" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        </div>
        <slot name="start" slot="start"></slot>
        <slot name="end" slot="end"></slot>
        <!--?lit$050605479$-->
      <slot></slot>
      <slot name="overline" slot="overline"></slot>
      <slot name="headline" slot="headline"></slot>
      <slot name="supporting-text" slot="supporting-text"></slot>
      <slot name="trailing-supporting-text" slot="trailing-supporting-text"></slot>
    
      </md-item>
    </li>
    </template>
    <span slot="headline"><!--?lit$050605479$-->Explain code</span>
  </md-menu-item><!---->
  </md-menu>
          <md-icon-button touch-target="none" data-aria-haspopup="menu" data-aria-expanded="false" aria-describedby="ai-menu-anchor-af5FKJF5mMLV-tooltip" data-aria-label="Available AI features" id="ai-menu-anchor-af5FKJF5mMLV" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Available AI features" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
          </md-icon-button>
          <colab-tooltip-trigger aria-hidden="true" for="ai-menu-anchor-af5FKJF5mMLV" id="ai-menu-anchor-af5FKJF5mMLV-tooltip" message="Available AI features"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Available AI features</div><!----><!--?--></template>
          </colab-tooltip-trigger><!----><!----> <md-icon-button touch-target="none" aria-describedby="button-copy-link-to-cell-tooltip" data-aria-label="Copy link to cell" command="copy-link-to-cell" id="button-copy-link-to-cell" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Copy link to cell">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->link</md-icon>
        <!--?lit$050605479$-->
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" for="button-copy-link-to-cell" id="button-copy-link-to-cell-tooltip" message="Copy link to cell"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Copy link to cell</div><!----><!--?--></template>
      </colab-tooltip-trigger><!----><!----> <md-icon-button touch-target="none" aria-describedby="button-add-comment-tooltip" data-aria-label="Add a comment
Ctrl+Alt+M" command="add-comment" id="button-add-comment" value="" style=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Add a comment
Ctrl+Alt+M">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->comment</md-icon>
        <!--?lit$050605479$-->
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" for="button-add-comment" id="button-add-comment-tooltip" message="Add a comment
Ctrl+Alt+M"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Add a comment</div><!----><!----><div><!--?lit$050605479$-->Ctrl+Alt+M</div><!----><!--?--></template>
      </colab-tooltip-trigger><!----><!----> <md-icon-button touch-target="none" aria-describedby="button-editor-preferences-tooltip" data-aria-label="Open editor settings" command="editor-preferences" id="button-editor-preferences" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Open editor settings">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon filled="" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->settings</md-icon>
        <!--?lit$050605479$-->
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" for="button-editor-preferences" id="button-editor-preferences-tooltip" message="Open editor settings"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Open editor settings</div><!----><!--?--></template>
      </colab-tooltip-trigger><!----><!----> <md-icon-button touch-target="none" aria-describedby="button-toggle-edit-markdown-tooltip" data-aria-label="Edit" command="toggle-edit-markdown" id="button-toggle-edit-markdown" toggle="" style="display: none;" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Edit" aria-pressed="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->edit</md-icon>
        <!--?lit$050605479$--><md-icon slot="selected" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->edit_off</md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" for="button-toggle-edit-markdown" id="button-toggle-edit-markdown-tooltip" message="Edit"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Edit</div><!----><!--?--></template>
      </colab-tooltip-trigger><!----><!----> <md-icon-button touch-target="none" aria-describedby="button-mirror-cell-in-tab-tooltip" data-aria-label="Mirror cell in tab" command="mirror-cell-in-tab" id="button-mirror-cell-in-tab" value="" style=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Mirror cell in tab">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$-->
      <g id="mirror-cell">
        <path d="M4,21V7H2V21a2,2,0,0,0,2,2H18V21Z"></path>
        <path d="M6,13v2H8.6L5,18.6,6.4,20,10,16.4V19h2V13Z"></path>
        <path d="M19,1H8A2,2,0,0,0,6,3v8H8V3H19V17H14v2h5a2,2,0,0,0,2-2V3A2,2,0,0,0,19,1Z"></path>
      </g></svg></md-icon>
        <!--?lit$050605479$-->
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" for="button-mirror-cell-in-tab" id="button-mirror-cell-in-tab-tooltip" message="Mirror cell in tab"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Mirror cell in tab</div><!----><!--?--></template>
      </colab-tooltip-trigger><!----><!----> <md-icon-button touch-target="none" aria-describedby="button-delete-cell-or-selection-tooltip" data-aria-label="Delete cell
Ctrl+M D" command="delete-cell-or-selection" id="button-delete-cell-or-selection" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Delete cell
Ctrl+M D">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->delete</md-icon>
        <!--?lit$050605479$-->
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" for="button-delete-cell-or-selection" id="button-delete-cell-or-selection-tooltip" message="Delete cell
Ctrl+M D"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Delete cell</div><!----><!----><div><!--?lit$050605479$-->Ctrl+M D</div><!----><!--?--></template>
      </colab-tooltip-trigger><!----><!--?lit$050605479$--><md-icon-button touch-target="none" data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-more-actions-tooltip" data-aria-label="More cell actions" class="cell-toolbar-more" id="button-more-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="More cell actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_vert</md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" for="button-more-actions" id="button-more-actions-tooltip" message="More cell actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->More cell actions</div><!----><!--?--></template>
      </colab-tooltip-trigger><!--?--></template></colab-cell-toolbar></div><div class="main-content" elevation="2"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale focused">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
1:03 AM (20 minutes ago)
executed in 3.503s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->1:03 AM (20 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 3.503s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><div class="editor flex monaco" data-keybinding-context="67" data-mode-id="notebook-python" style="height: 333px; --vscode-editorCodeLens-lineHeight: 16px; --vscode-editorCodeLens-fontSize: 12px; --vscode-editorCodeLens-fontFeatureSettings: &quot;liga&quot; off, &quot;calt&quot; off;"><div class="monaco-editor no-user-select  showUnused showDeprecated vs-dark" role="code" data-uri="inmemory://model/29" style="width: 1192px; height: 333px;"><div data-mprt="3" class="overflow-guard" style="width: 1192px; height: 333px; overflow: clip;"><div class="margin" role="presentation" aria-hidden="true" style="position: absolute; contain: strict; will-change: unset; top: 0px; height: 333px; width: 6px;"><div class="glyph-margin" style="left: 0px; width: 0px; height: 333px;"></div><div class="margin-view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="margin-view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 6px; height: 333px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line current-line-margin-both" style="width:6px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div></div><div class="glyph-margin-widgets" style="position: absolute; top: 0px;"></div></div><div class="monaco-scrollable-element editor-scrollable vs-dark" role="presentation" data-mprt="5" style="position: absolute; overflow: hidden; left: 6px; width: 1186px; height: 333px;"><div class="lines-content monaco-editor-background" style="position: absolute; overflow: hidden; width: 1e+06px; height: 333px; contain: strict; will-change: unset; top: 0px; left: 0px;"><div class="view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; height: 0px; width: 1484px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line" style="width:1484px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div></div><div role="presentation" aria-hidden="true" class="view-rulers"><div class="view-ruler" style="width: 2px; height: 333px; left: 615.938px;"></div></div><div class="view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="view-lines monaco-mouse-cursor-text" role="presentation" aria-hidden="true" data-mprt="7" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 1484px; height: 333px;"><div style="top:0px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Create&nbsp;a&nbsp;dashboard&nbsp;with&nbsp;subplots</span></span></div><div style="top:19px;height:19px;" class="view-line"><span><span class="mtk1">dashboard&nbsp;=&nbsp;make_subplots</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">rows=</span><span class="mtk6">3</span><span class="mtk12">,</span><span class="mtk1">&nbsp;cols=</span><span class="mtk6">2</span><span class="mtk12">,</span><span class="mtk1">&nbsp;subplot_titles=</span><span class="mtk12 bracket-highlighting-1">(</span><span class="mtk5">"Trip&nbsp;Duration&nbsp;Distribution"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">"Daily&nbsp;Trip&nbsp;Patterns"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">"Popular&nbsp;Start&nbsp;Stations"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">"User&nbsp;Age&nbsp;Distribution"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">"User&nbsp;Age&nbsp;by&nbsp;User&nbsp;Type"</span><span class="mtk12 bracket-highlighting-1">)</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:38px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:57px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Add&nbsp;each&nbsp;figure&nbsp;to&nbsp;the&nbsp;dashboard</span></span></div><div style="top:76px;height:19px;" class="view-line"><span><span class="mtk1">dashboard.add_trace</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">fig1.data</span><span class="mtk12 bracket-highlighting-1">[</span><span class="mtk6">0</span><span class="mtk12 bracket-highlighting-1">]</span><span class="mtk12">,</span><span class="mtk1">&nbsp;row=</span><span class="mtk6">1</span><span class="mtk12">,</span><span class="mtk1">&nbsp;col=</span><span class="mtk6">1</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:95px;height:19px;" class="view-line"><span><span class="mtk1">dashboard.add_trace</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">fig1.data</span><span class="mtk12 bracket-highlighting-1">[</span><span class="mtk6">1</span><span class="mtk12 bracket-highlighting-1">]</span><span class="mtk12">,</span><span class="mtk1">&nbsp;row=</span><span class="mtk6">1</span><span class="mtk12">,</span><span class="mtk1">&nbsp;col=</span><span class="mtk6">1</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:114px;height:19px;" class="view-line"><span><span class="mtk1">dashboard.add_trace</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">fig2.data</span><span class="mtk12 bracket-highlighting-1">[</span><span class="mtk6">0</span><span class="mtk12 bracket-highlighting-1">]</span><span class="mtk12">,</span><span class="mtk1">&nbsp;row=</span><span class="mtk6">1</span><span class="mtk12">,</span><span class="mtk1">&nbsp;col=</span><span class="mtk6">2</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:133px;height:19px;" class="view-line"><span><span class="mtk1">dashboard.add_trace</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">fig3.data</span><span class="mtk12 bracket-highlighting-1">[</span><span class="mtk6">0</span><span class="mtk12 bracket-highlighting-1">]</span><span class="mtk12">,</span><span class="mtk1">&nbsp;row=</span><span class="mtk6">2</span><span class="mtk12">,</span><span class="mtk1">&nbsp;col=</span><span class="mtk6">1</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:152px;height:19px;" class="view-line"><span><span class="mtk1">dashboard.add_trace</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">fig4.data</span><span class="mtk12 bracket-highlighting-1">[</span><span class="mtk6">0</span><span class="mtk12 bracket-highlighting-1">]</span><span class="mtk12">,</span><span class="mtk1">&nbsp;row=</span><span class="mtk6">2</span><span class="mtk12">,</span><span class="mtk1">&nbsp;col=</span><span class="mtk6">2</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:171px;height:19px;" class="view-line"><span><span class="mtk1">dashboard.add_trace</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">fig5.data</span><span class="mtk12 bracket-highlighting-1">[</span><span class="mtk6">0</span><span class="mtk12 bracket-highlighting-1">]</span><span class="mtk12">,</span><span class="mtk1">&nbsp;row=</span><span class="mtk6">3</span><span class="mtk12">,</span><span class="mtk1">&nbsp;col=</span><span class="mtk6">1</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:190px;height:19px;" class="view-line"><span><span class="mtk1">dashboard.add_trace</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">fig5.data</span><span class="mtk12 bracket-highlighting-1">[</span><span class="mtk6">1</span><span class="mtk12 bracket-highlighting-1">]</span><span class="mtk12">,</span><span class="mtk1">&nbsp;row=</span><span class="mtk6">3</span><span class="mtk12">,</span><span class="mtk1">&nbsp;col=</span><span class="mtk6">1</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:209px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:228px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Update&nbsp;layout&nbsp;for&nbsp;the&nbsp;dashboard</span></span></div><div style="top:247px;height:19px;" class="view-line"><span><span class="mtk1">dashboard.update_layout</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">height=</span><span class="mtk6">1200</span><span class="mtk12">,</span><span class="mtk1">&nbsp;width=</span><span class="mtk6">1000</span><span class="mtk12">,</span><span class="mtk1">&nbsp;title_text=</span><span class="mtk5">"Ford&nbsp;GoBike&nbsp;Trip&nbsp;Data&nbsp;Dashboard"</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:266px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:285px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Display&nbsp;the&nbsp;dashboard</span></span></div><div style="top:304px;height:19px;" class="view-line"><span><span class="mtk1">dashboard.show</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span></span></div></div><div data-mprt="1" class="contentWidgets" style="position: absolute; top: 0px;"></div><div role="presentation" aria-hidden="true" class="cursors-layer cursor-line-style cursor-solid"><div class="cursor monaco-mouse-cursor-text " style="height: 19px; top: 0px; left: 0px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; display: block; visibility: hidden; padding-left: 0px; width: 1.6px;"></div></div></div><div role="presentation" aria-hidden="true" class="visible scrollbar horizontal" style="position: absolute; width: 1172px; height: 10px; left: 0px; bottom: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; width: 936px;"></div></div><canvas class="decorationsOverviewRuler" aria-hidden="true" width="17" height="416" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; top: 0px; right: 0px; width: 14px; height: 333px; will-change: unset; display: block;"></canvas><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute; width: 14px; height: 333px; right: 0px; top: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 14px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; height: 333px;"></div></div></div><div role="presentation" aria-hidden="true" style="width: 1192px;"></div><textarea data-mprt="6" class="inputarea monaco-mouse-cursor-text" wrap="on" autocorrect="off" autocapitalize="off" autocomplete="off" spellcheck="false" aria-label="Editor content;Press Alt+F1 for Accessibility Options." tabindex="0" role="textbox" aria-roledescription="editor" aria-multiline="true" aria-haspopup="false" aria-autocomplete="both" style="tab-size: 15.3984px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; top: 0px; left: 6px; width: 76992px; height: 1px;"></textarea><div class="monaco-editor-background textAreaCover" style="position: absolute; top: 0px; left: 0px; width: 0px; height: 0px;"></div><div data-mprt="4" class="overlayWidgets" style="width: 1192px;"><div widgetid="editor.contrib.quickInputWidget" style="position: absolute; top: 0px; right: 50%;"></div></div><div data-mprt="8" class="minimap slider-mouseover" role="presentation" aria-hidden="true" style="position: absolute; left: 0px; width: 0px; height: 333px;"><div class="minimap-shadow-hidden" style="height: 333px;"></div><canvas width="0" height="416" style="position: absolute; left: 0px; width: 0px; height: 333px;"></canvas><canvas class="minimap-decorations-layer" width="0" height="416" style="position: absolute; left: 0px; width: 0px; height: 333px;"></canvas><div class="minimap-slider" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; width: 0px; will-change: unset;"><div class="minimap-slider-horizontal" style="position: absolute; width: 0px; height: 0px;"></div></div></div><div role="presentation" aria-hidden="true" class="blockDecorations-container"></div></div><div data-mprt="2" class="overflowingContentWidgets"><div widgetid="editor.contrib.resizableContentHoverWidget" style="position: fixed; height: 10px; width: 10px; z-index: 50; display: none; visibility: hidden; max-width: 1536px;"><div class="monaco-sash vertical" style="left: 8px;"></div><div class="monaco-sash vertical" style="left: -2px;"></div><div class="monaco-sash orthogonal-edge-north horizontal" style="top: -2px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-sash orthogonal-edge-south horizontal" style="top: 8px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-hover hidden" role="tooltip" tabindex="0"><div class="monaco-scrollable-element " role="presentation" style="position: relative; overflow: hidden;"><div class="monaco-hover-content" style="overflow: hidden; font-size: 14px; line-height: 1.35714; max-width: 786.72px; max-height: 250px;"></div><div role="presentation" aria-hidden="true" class="invisible scrollbar horizontal" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div class="shadow"></div><div class="shadow"></div><div class="shadow"></div></div></div></div></div><div class=".in-cell-overflowing"></div></div></div></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 25 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div class="outputview" style="height: 1000px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals" src="./Untitled21.ipynb - Colab_files/outputframe(8).html" class="" style="height: 1000px;"></iframe></div></div><div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling" id="cell-gQlfxxu4mOiA" role="region" aria-label="Cell 26: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
1:06 AM (18 minutes ago)
executed in 4.169s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->1:06 AM (18 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 4.169s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark" data-lang="notebook-python"><span><span class="mtk18">import</span><span class="mtk1">&nbsp;plotly.express&nbsp;</span><span class="mtk18">as</span><span class="mtk1">&nbsp;px</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$050605479$-->Start coding or <span role="button" class="link" tabindex="0">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 26 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div><colab-static-output-renderer role="group" tabindex="0"><div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling code-has-output" id="cell-vUk2Lx7Om8n1" role="region" aria-label="Cell 27: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
1:06 AM (17 minutes ago)
executed in 4.465s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->1:06 AM (17 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 4.465s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark" data-lang="notebook-python"><span><span class="mtk1">fig&nbsp;=&nbsp;px.box</span><span class="mtk12">(</span><span class="mtk1">df</span><span class="mtk12">,</span><span class="mtk1">&nbsp;x=</span><span class="mtk5">"user_type"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;y=</span><span class="mtk5">"duration_min"</span><span class="mtk12">,</span><span class="mtk1">&nbsp;title=</span><span class="mtk5">"Trip&nbsp;Duration&nbsp;Distribution&nbsp;by&nbsp;User&nbsp;Type"</span><span class="mtk12">)</span></span><br><span><span class="mtk1">fig.show</span><span class="mtk12">()</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$050605479$-->Start coding or <span role="button" class="link" tabindex="0">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 27 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div class="outputview" style="height: 542px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals" src="./Untitled21.ipynb - Colab_files/outputframe(9).html" class="" style="height: 542px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling code-has-output" id="cell-KE71b1lGm7jO" role="region" aria-label="Cell 28: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
1:06 AM (17 minutes ago)
executed in 0.148s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->1:06 AM (17 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 0.148s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark colab-dark" data-lang="notebook-python"><span><span class="mtk1">trips_per_day&nbsp;=&nbsp;df.groupby</span><span class="mtk12">(</span><span class="mtk5">'day_of_week'</span><span class="mtk12">)[</span><span class="mtk5">'start_time'</span><span class="mtk12">]</span><span class="mtk1">.count</span><span class="mtk12">()</span><span class="mtk1">.reindex</span><span class="mtk12">([</span><span class="mtk5">'Monday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Tuesday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Wednesday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Thursday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Friday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Saturday'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'Sunday'</span><span class="mtk12">])</span></span><br><span><span class="mtk1">fig&nbsp;=&nbsp;px.line</span><span class="mtk12">(</span><span class="mtk1">x=trips_per_day.index</span><span class="mtk12">,</span><span class="mtk1">&nbsp;y=trips_per_day.values</span><span class="mtk12">,</span><span class="mtk1">&nbsp;title=</span><span class="mtk5">'Daily&nbsp;Trip&nbsp;Patterns'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;labels=</span><span class="mtk12">{</span><span class="mtk5">'x'</span><span class="mtk12">:</span><span class="mtk5">'Day&nbsp;of&nbsp;the&nbsp;Week'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'y'</span><span class="mtk12">:</span><span class="mtk5">'Number&nbsp;of&nbsp;Trips'</span><span class="mtk12">})</span></span><br><span><span class="mtk1">fig.show</span><span class="mtk12">()</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$050605479$-->Start coding or <span role="button" class="link" tabindex="0">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 28 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div class="outputview" style="height: 542px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals" src="./Untitled21.ipynb - Colab_files/outputframe(10).html" class="" style="height: 542px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling code-has-output" id="cell-zSqNeXpUnDQV" role="region" aria-label="Cell 29: Code cell: " style="opacity: 1;" tabindex="-1"><div class="agent-focus-label">
      <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>spark</md-icon>
      <!--?lit$050605479$-->Gemini
    </div><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea-and-title">
        <!-- The colab-form-title element is injected here, if it exists. -->
        <div class="inputarea horizontal layout code">
          <div class="cell-gutter">
            <!-- Bounding range for vertical scrolling of icons -->
            <div class="cell-execution-container">
              <colab-run-button><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <button id="run-button" aria-describedby="run-button-tooltip" aria-label="Run cell" aria-disabled="false">
        <!--?lit$050605479$--><span class="execution-count"><!--?lit$050605479$-->[ ]</span>
        <span aria-hidden="true" class="cell-execution-indicator"><!--?lit$050605479$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$050605479$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg></span>
      </button>
      <!--?lit$050605479$--><colab-tooltip-trigger for="run-button" id="run-button-tooltip" aria-hidden="true" message="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by Maryam Sayed
1:07 AM (17 minutes ago)
executed in 0.142s"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Run cell (Ctrl+Enter)</div><!----><!----><div><!--?lit$050605479$-->cell has not been executed in this session</div><!----><!----><br><!----><!----><div><!--?lit$050605479$-->executed by Maryam Sayed</div><!----><!----><div><!--?lit$050605479$-->1:07 AM (17 minutes ago)</div><!----><!----><div><!--?lit$050605479$-->executed in 0.142s</div><!----><!--?--></template>
    </colab-tooltip-trigger>
      <!--?lit$050605479$--><!--?-->
    </div></template></colab-run-button>
            </div>
          </div>
        <div class="editor flex lazy-editor" style=""><div class="editor flex monaco" data-keybinding-context="133" data-mode-id="notebook-python" style="height: 67px; --vscode-editorCodeLens-lineHeight: 16px; --vscode-editorCodeLens-fontSize: 12px; --vscode-editorCodeLens-fontFeatureSettings: &quot;liga&quot; off, &quot;calt&quot; off;"><div class="monaco-editor no-user-select  showUnused showDeprecated vs-dark" role="code" data-uri="inmemory://model/33" style="width: 1192px; height: 67px;"><div data-mprt="3" class="overflow-guard" style="width: 1192px; height: 67px; overflow: clip;"><div class="margin" role="presentation" aria-hidden="true" style="position: absolute; contain: strict; will-change: unset; top: 0px; height: 67px; width: 6px;"><div class="glyph-margin" style="left: 0px; width: 0px; height: 67px;"></div><div class="margin-view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="margin-view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 6px; height: 67px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line current-line-margin-both" style="width:6px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div></div><div class="glyph-margin-widgets" style="position: absolute; top: 0px;"></div></div><div class="monaco-scrollable-element editor-scrollable vs-dark" role="presentation" data-mprt="5" style="position: absolute; overflow: hidden; left: 6px; width: 1186px; height: 67px;"><div class="lines-content monaco-editor-background" style="position: absolute; overflow: hidden; width: 1e+06px; height: 67px; contain: strict; will-change: unset; top: 0px; left: 0px;"><div class="view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; height: 0px; width: 1553px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line" style="width:1553px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div></div><div role="presentation" aria-hidden="true" class="view-rulers"><div class="view-ruler" style="width: 2px; height: 67px; left: 615.938px;"></div></div><div class="view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="view-lines monaco-mouse-cursor-text" role="presentation" aria-hidden="true" data-mprt="7" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 1553px; height: 67px;"><div style="top:0px;height:19px;" class="view-line"><span><span class="mtk1">popular_start_stations&nbsp;=&nbsp;df</span><span class="mtk12 bracket-highlighting-0">[</span><span class="mtk5">'start_station_name'</span><span class="mtk12 bracket-highlighting-0">]</span><span class="mtk1">.value_counts</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span><span class="mtk1">.head</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk6">10</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:19px;height:19px;" class="view-line"><span><span class="mtk1">fig&nbsp;=&nbsp;px.bar</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk1">y=popular_start_stations.index</span><span class="mtk12">,</span><span class="mtk1">&nbsp;x=popular_start_stations.values</span><span class="mtk12">,</span><span class="mtk1">&nbsp;orientation=</span><span class="mtk5">'h'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;title=</span><span class="mtk5">'Top&nbsp;10&nbsp;Most&nbsp;Popular&nbsp;Start&nbsp;Stations'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;labels=</span><span class="mtk12 bracket-highlighting-1">{</span><span class="mtk5">'y'</span><span class="mtk12">:</span><span class="mtk5">'Start&nbsp;Station&nbsp;Name'</span><span class="mtk12">,</span><span class="mtk1">&nbsp;</span><span class="mtk5">'x'</span><span class="mtk12">:</span><span class="mtk5">'Number&nbsp;of&nbsp;Trips'</span><span class="mtk12 bracket-highlighting-1">}</span><span class="mtk12 bracket-highlighting-0">)</span></span></div><div style="top:38px;height:19px;" class="view-line"><span><span class="mtk1">fig.show</span><span class="mtk12 bracket-highlighting-0">(</span><span class="mtk12 bracket-highlighting-0">)</span></span></div></div><div data-mprt="1" class="contentWidgets" style="position: absolute; top: 0px;"></div><div role="presentation" aria-hidden="true" class="cursors-layer cursor-line-style cursor-solid"><div class="cursor monaco-mouse-cursor-text " style="height: 19px; top: 0px; left: 0px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; display: block; visibility: hidden; padding-left: 0px; width: 1.6px;"></div></div></div><div role="presentation" aria-hidden="true" class="visible scrollbar horizontal" style="position: absolute; width: 1172px; height: 10px; left: 0px; bottom: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; width: 895px;"></div></div><canvas class="decorationsOverviewRuler" aria-hidden="true" width="17" height="83" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; top: 0px; right: 0px; width: 14px; height: 67px; will-change: unset; display: block;"></canvas><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute; width: 14px; height: 67px; right: 0px; top: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 14px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; height: 67px;"></div></div></div><div role="presentation" aria-hidden="true" style="width: 1192px;"></div><textarea data-mprt="6" class="inputarea monaco-mouse-cursor-text" wrap="on" autocorrect="off" autocapitalize="off" autocomplete="off" spellcheck="false" aria-label="Editor content;Press Alt+F1 for Accessibility Options." tabindex="0" role="textbox" aria-roledescription="editor" aria-multiline="true" aria-haspopup="false" aria-autocomplete="both" style="tab-size: 15.3984px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; top: 0px; left: 6px; width: 76992px; height: 1px;"></textarea><div class="monaco-editor-background textAreaCover" style="position: absolute; top: 0px; left: 0px; width: 0px; height: 0px;"></div><div data-mprt="4" class="overlayWidgets" style="width: 1192px;"></div><div data-mprt="8" class="minimap slider-mouseover" role="presentation" aria-hidden="true" style="position: absolute; left: 0px; width: 0px; height: 67px;"><div class="minimap-shadow-hidden" style="height: 67px;"></div><canvas width="0" height="83" style="position: absolute; left: 0px; width: 0px; height: 67px;"></canvas><canvas class="minimap-decorations-layer" width="0" height="83" style="position: absolute; left: 0px; width: 0px; height: 67px;"></canvas><div class="minimap-slider" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; width: 0px; will-change: unset;"><div class="minimap-slider-horizontal" style="position: absolute; width: 0px; height: 0px;"></div></div></div><div role="presentation" aria-hidden="true" class="blockDecorations-container"></div></div><div data-mprt="2" class="overflowingContentWidgets" style="display: none;"><div widgetid="editor.contrib.resizableContentHoverWidget" style="position: fixed; height: 10px; width: 10px; z-index: 50; display: none; visibility: hidden; max-width: 1536px;"><div class="monaco-sash vertical" style="left: 8px;"></div><div class="monaco-sash vertical" style="left: -2px;"></div><div class="monaco-sash orthogonal-edge-north horizontal" style="top: -2px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-sash orthogonal-edge-south horizontal" style="top: 8px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-hover hidden" tabindex="0" role="tooltip"><div class="monaco-scrollable-element " role="presentation" style="position: relative; overflow: hidden;"><div class="monaco-hover-content" style="overflow: hidden; font-size: 14px; line-height: 1.35714; max-width: 786.72px; max-height: 250px;"></div><div role="presentation" aria-hidden="true" class="invisible scrollbar horizontal" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div class="shadow"></div><div class="shadow"></div><div class="shadow"></div></div></div></div></div><div class=".in-cell-overflowing"><div widgetid="editor.contrib.quickInputWidget" style="position: absolute; top: 0px; right: 50%;"></div></div></div></div></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
      </div>
    <div class="output" aria-label="Cell 29 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info><template shadowrootmode="open"><!----><md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" aria-describedby="button-output-actions-tooltip" data-aria-label="Code cell output actions" id="button-output-actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button>
      <colab-tooltip-trigger aria-hidden="true" id="button-output-actions-tooltip" for="button-output-actions" message="Code cell output actions"><template shadowrootmode="open"><!----><!--?lit$050605479$--><!----><div><!--?lit$050605479$-->Code cell output actions</div><!----><!--?--></template></colab-tooltip-trigger></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer" style="min-height: 0px;"> <div><div class="outputview" style="height: 542px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals" src="./Untitled21.ipynb - Colab_files/outputframe(11).html" class="" style="height: 542px;"></iframe></div></div><div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" data-aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" data-aria-label="Add text cell" title="Add text cell" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$050605479$-->Text
        </md-outlined-button>
        <!--?lit$050605479$-->
      </div><hr>
    </div></div></div>
              </div>
            </div>
          <section class="sidebar" aria-label="Comments" style="display: none;"></section></div>
          <!--?lit$050605479$--> <div class="footer-links">
      <a target="_blank" href="https://colab.research.google.com/signup?utm_source=footer&amp;utm_medium=link&amp;utm_campaign=footer_links">
        <!--?lit$050605479$-->Colab paid products
      </a>
      -
      <a href="https://colab.research.google.com/cancel-subscription" target="_blank">
        <!--?lit$050605479$-->Cancel contracts here
      </a>
    </div>
        </div>
      </colab-shaded-scroller>
      <div class="notebook-scroll-shadow" style="box-shadow: rgba(0, 0, 0, 0.15) 0px 4px 4px -2px inset;"></div>
    </div></colab-tab></div>
  </div></colab-tab-pane>
      <colab-resizer style="height: 33.3%" class="sn-resize no-tabs"><div class="resizer-thumb"></div>
        <!--?lit$050605479$--><colab-tab-pane class="layout vertical grow no-tabs" align="horizontal"><!----> <div class="layout vertical grow">
    <div class="tab-pane-header layout horizontal noshrink">
      <md-tabs><template shadowrootmode="open"><!---->
      <div class="tabs">
        <slot></slot>
      </div>
      <md-divider part="divider"><template shadowrootmode="open"><!----></template></md-divider>
    </template></md-tabs>
      <div class="layout grow"></div>
      <!--?lit$050605479$--> <md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" title="More tab actions" data-aria-label="More tab actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="More tab actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
    <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_horiz</md-icon>
  </md-icon-button>
    </div>
    <div class="layout vertical grow tab-pane-container"> </div>
  </div></colab-tab-pane>
      </colab-resizer>
    </div>
      <colab-resizer style="width: 37%" class="we-resize no-tabs"><div class="resizer-thumb"></div>
        <!--?lit$050605479$--> <div class="layout vertical tab-pane-parent">
      <!--?lit$050605479$--><colab-tab-pane class="layout vertical grow no-tabs" align="horizontal"><!----> <div class="layout vertical grow">
    <div class="tab-pane-header layout horizontal noshrink">
      <md-tabs><template shadowrootmode="open"><!---->
      <div class="tabs">
        <slot></slot>
      </div>
      <md-divider part="divider"><template shadowrootmode="open"><!----></template></md-divider>
    </template></md-tabs>
      <div class="layout grow"></div>
      <!--?lit$050605479$--> <md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" title="More tab actions" data-aria-label="More tab actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="More tab actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
    <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_horiz</md-icon>
  </md-icon-button>
    </div>
    <div class="layout vertical grow tab-pane-container"> </div>
  </div></colab-tab-pane>
      <colab-resizer style="height: 33.3%" class="sn-resize no-tabs"><div class="resizer-thumb"></div>
        <!--?lit$050605479$--><colab-tab-pane class="layout vertical grow no-tabs" align="horizontal"><!----> <div class="layout vertical grow">
    <div class="tab-pane-header layout horizontal noshrink">
      <md-tabs><template shadowrootmode="open"><!---->
      <div class="tabs">
        <slot></slot>
      </div>
      <md-divider part="divider"><template shadowrootmode="open"><!----></template></md-divider>
    </template></md-tabs>
      <div class="layout grow"></div>
      <!--?lit$050605479$--> <md-icon-button data-aria-expanded="false" data-aria-haspopup="menu" title="More tab actions" data-aria-label="More tab actions" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="More tab actions" aria-haspopup="menu" aria-expanded="false">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
    <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_horiz</md-icon>
  </md-icon-button>
    </div>
    <div class="layout vertical grow tab-pane-container"> </div>
  </div></colab-tab-pane>
      </colab-resizer>
    </div>
      </colab-resizer>
    </div></colab-tab-layout-container>
        </div>
        <div class="proxies"><div><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation" src="./Untitled21.ipynb - Colab_files/outputframe(12).html" style="width: 1px; height: 1px; position: absolute; top: -100px;"></iframe></div><div><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals" src="./Untitled21.ipynb - Colab_files/outputframe(13).html" style="width: 1px; height: 1px; position: absolute; top: -100px;"></iframe></div></div>
      <colab-file-viewer-manager></colab-file-viewer-manager></div>
    <colab-status-bar role="region" aria-label="Runtime status bar" style="min-height: inherit;"><template shadowrootmode="open"><!----><!--?lit$050605479$--> <!--?lit$050605479$--> <div class="cell-status">
        <button><!--?lit$050605479$--><md-icon class="success" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$--><svg viewBox="0 0 24 24"><!--?lit$050605479$--><path d="M9 16.17L4.83 12l-1.42 1.41L9 19 21 7l-1.41-1.41z"></path></svg></md-icon>&nbsp; <!--?lit$050605479$-->7m 1s</button>
        <button title="Show executed code history

1:38 AM (9 minutes ago)
executed in 421.191s"><!--?lit$050605479$-->completed at 1:38 AM</button>
      </div>
      <md-icon-button class="visible-on-closed" title="Connected" disabled="" value="" data-aria-label="Connected"><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Connected" disabled="">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple disabled="" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon filled="" class="visible-on-closed" status="icon-okay" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$050605479$-->fiber_manual_record</md-icon>
      </md-icon-button>
      <!--?lit$050605479$-->
      <md-icon-button title="Close" data-aria-label="Close" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Close">
        <!--?lit$050605479$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$050605479$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$050605479$--><span class="icon"><slot></slot></span>
        <!--?lit$050605479$-->
        <!--?lit$050605479$--><span class="touch"></span>
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>close</md-icon>
      </md-icon-button></template></colab-status-bar></div><div class="goog-menu colab-styled-scroller" id="file-menu" role="menu" aria-haspopup="true" style="user-select: none; max-height: 628px; visibility: visible; left: 68px; top: 62px; display: none;" aria-activedescendant="download-submenu-menu-button"><!--?lit$050605479$--><div command="locate-in-drive" class="goog-menuitem" role="menuitem" id=":2" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Locate in Drive<!--?lit$050605479$--></div></div><div command="open-in-playground" class="goog-menuitem" role="menuitem" id=":3" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Open in playground mode<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":4" style="user-select: none;"></div><div command="new" class=" goog-menuitem " role="menuitem" id=":5" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->New notebook in Drive<!--?lit$050605479$--></div></div><div command="open" class="goog-menuitem" role="menuitem" id=":6" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Open notebook<!--?lit$050605479$--><span class="goog-menuitem-accel">Ctrl+O</span></div></div><div command="import-notebook" class="goog-menuitem" role="menuitem" id=":7" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Upload notebook<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":8" style="user-select: none;"></div><div command="rename" class="goog-menuitem" role="menuitem" id=":9" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Rename<!--?lit$050605479$--></div></div><div command="move-notebook" class="goog-menuitem" role="menuitem" id=":a" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Move<!--?lit$050605479$--></div></div><div command="trash" class="goog-menuitem" role="menuitem" id=":b" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Move to trash<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":c" style="user-select: none;"></div><div command="clone" class="goog-menuitem" role="menuitem" id=":d" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Save a copy in Drive<!--?lit$050605479$--></div></div><div command="copy-to-gist" class="goog-menuitem" role="menuitem" id=":e" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Save a copy as a GitHub Gist<!--?lit$050605479$--></div></div><div command="copy-to-github" class="goog-menuitem" role="menuitem" id=":f" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Save a copy in GitHub<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":g" style="user-select: none;"></div><div command="save" class="goog-menuitem" role="menuitem" id=":h" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Save<!--?lit$050605479$--><span class="goog-menuitem-accel">Ctrl+S</span></div></div><div command="save-and-checkpoint" class="goog-menuitem" role="menuitem" id=":i" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Save and pin revision<!--?lit$050605479$--><span class="goog-menuitem-accel">Ctrl+M S</span></div></div><div command="show-history" class="goog-menuitem" role="menuitem" id=":j" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Revision history<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":k" style="user-select: none;"></div><div class="goog-submenu goog-menuitem goog-menuitem-highlight" id="download-submenu-menu-button" role="menuitem" aria-haspopup="true" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;">
      <!--?lit$050605479$-->Download
    <span class="goog-submenu-arrow" style="user-select: none;">►</span></div></div><div command="print" class="goog-menuitem" role="menuitem" id=":o" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Print<!--?lit$050605479$--><span class="goog-menuitem-accel">Ctrl+P</span></div></div></div><div class="goog-menu" id="download-submenu-menu" role="menu" aria-haspopup="true" style="user-select: none; left: 395.8px; top: 581.8px; display: none;"><!--?lit$050605479$--><div command="download-ipynb" class="goog-menuitem" role="menuitem" id=":m" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Download .ipynb<!--?lit$050605479$--></div></div><div command="download-python" class=" goog-menuitem " role="menuitem" id=":n" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Download .py<!--?lit$050605479$--></div></div></div><div class="goog-menu" id="edit-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$050605479$--><div command="undo" class=" goog-menuitem " role="menuitem" id=":q" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Undo<!--?lit$050605479$--></div></div><div command="redo" class=" goog-menuitem " role="menuitem" id=":r" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Redo<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":s" style="user-select: none;"></div><div command="select-all" class=" goog-menuitem " role="menuitem" id=":t" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Select all cells<!--?lit$050605479$--></div></div><div command="cut" class=" goog-menuitem " role="menuitem" id=":u" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Cut cell or selection<!--?lit$050605479$--></div></div><div command="copy" class=" goog-menuitem " role="menuitem" id=":v" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Copy cell or selection<!--?lit$050605479$--></div></div><div command="paste" class=" goog-menuitem " role="menuitem" id=":w" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Paste<!--?lit$050605479$--></div></div><div command="delete-cell-or-selection" class=" goog-menuitem " role="menuitem" id=":x" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Delete selected cells<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":y" style="user-select: none;"></div><div command="find" class=" goog-menuitem " role="menuitem" id=":z" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Find and replace<!--?lit$050605479$--></div></div><div command="find-next" class=" goog-menuitem " role="menuitem" id=":10" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Find next<!--?lit$050605479$--></div></div><div command="find-previous" class=" goog-menuitem " role="menuitem" id=":11" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Find previous<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":12" style="user-select: none;"></div><div command="notebook-settings" class=" goog-menuitem " role="menuitem" id=":13" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Notebook settings<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":14" style="user-select: none;"></div><div command="clear-outputs" class=" goog-menuitem " role="menuitem" id=":15" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Clear all outputs<!--?lit$050605479$--></div></div></div><div class="goog-menu" id="view-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$050605479$--><div command="show-toc-pane" class="goog-menuitem goog-option" role="menuitemcheckbox" aria-checked="false" id=":17" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><div class="goog-menuitem-checkbox" style="user-select: none;"><!----><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>check</md-icon> </div><!--?lit$050605479$-->Table of contents<!--?lit$050605479$--></div></div><div command="show-fileinfo" class=" goog-menuitem " role="menuitem" id=":18" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Notebook info<!--?lit$050605479$--></div></div><div command="show-executedcode" class=" goog-menuitem " role="menuitem" id=":19" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Executed code history<!--?lit$050605479$--></div></div><div class="goog-submenu goog-menuitem" id="comments-submenu-menu-button" role="menuitem" aria-haspopup="true" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;">
      <!--?lit$050605479$-->Comments
    <span class="goog-submenu-arrow" style="user-select: none;">►</span></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":1e" style="user-select: none;"></div><div command="collapse-sections" class=" goog-menuitem " role="menuitem" id=":1f" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Collapse sections<!--?lit$050605479$--></div></div><div command="expand-sections" class=" goog-menuitem " role="menuitem" id=":1g" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Expand sections<!--?lit$050605479$--></div></div><div command="save-section-layout" class=" goog-menuitem " role="menuitem" id=":1h" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Save collapsed section layout<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":1i" style="user-select: none;"></div><div command="hide-code" class=" goog-menuitem " role="menuitem" id=":1j" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Show/hide code<!--?lit$050605479$--></div></div><div command="toggle-output" class=" goog-menuitem " role="menuitem" id=":1k" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Show/hide output<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":1l" style="user-select: none;"></div><div command="focus-next-tab" class=" goog-menuitem " role="menuitem" id=":1m" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Focus next tab<!--?lit$050605479$--></div></div><div command="focus-previous-tab" class=" goog-menuitem " role="menuitem" id=":1n" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Focus previous tab<!--?lit$050605479$--></div></div><div command="move-tab-to-next" class=" goog-menuitem " role="menuitem" id=":1o" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Move tab to next pane<!--?lit$050605479$--></div></div><div command="move-tab-to-prev" class=" goog-menuitem " role="menuitem" id=":1p" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Move tab to previous pane<!--?lit$050605479$--></div></div></div><div class="goog-menu" id="comments-submenu-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$050605479$--><div command="hide-sidebar-comments" class=" goog-menuitem goog-option-selectable " role="menuitem" id=":1b" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Hide comments<!--?lit$050605479$--></div></div><div command="show-minimized-sidebar-comments" class=" goog-menuitem goog-option-selectable " role="menuitem" id=":1c" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Minimize comments<!--?lit$050605479$--></div></div><div command="show-expanded-sidebar-comments" class=" goog-menuitem goog-option-selectable " role="menuitem" id=":1d" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Expand comments<!--?lit$050605479$--></div></div></div><div class="goog-menu" id="insert-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$050605479$--><div command="insert-cell-below" class=" goog-menuitem " role="menuitem" id=":1r" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Code cell<!--?lit$050605479$--></div></div><div command="add-text" class=" goog-menuitem " role="menuitem" id=":1s" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Text cell<!--?lit$050605479$--></div></div><div command="add-section-header" class=" goog-menuitem " role="menuitem" id=":1t" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Section header cell<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":1u" style="user-select: none;"></div><div command="open-scratch-code-cell" class=" goog-menuitem " role="menuitem" id=":1v" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Scratch code cell<!--?lit$050605479$--></div></div><div command="snippets" class=" goog-menuitem " role="menuitem" id=":1w" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Code snippets<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":1x" style="user-select: none;"></div><div command="add-form-field" class=" goog-menuitem " role="menuitem" id=":1y" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Add a form field<!--?lit$050605479$--></div></div></div><div class="goog-menu colab-styled-scroller" id="runtime-menu" role="menu" aria-haspopup="true" style="user-select: none; max-height: 628px; visibility: visible; left: 249.975px; top: 62px; display: none;"><!--?lit$050605479$--><div command="runall" class="goog-menuitem" role="menuitem" id=":20" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Run all<!--?lit$050605479$--><span class="goog-menuitem-accel">Ctrl+F9</span></div></div><div command="runbefore" class="goog-menuitem goog-menuitem-disabled" role="menuitem" id=":21" aria-disabled="true" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Run before<!--?lit$050605479$--><span class="goog-menuitem-accel">Ctrl+F8</span></div></div><div command="runfocused" class="goog-menuitem" role="menuitem" id=":22" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Run the focused cell<!--?lit$050605479$--><span class="goog-menuitem-accel">Ctrl+Enter</span></div></div><div command="runselected" class="goog-menuitem" role="menuitem" id=":23" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Run selection<!--?lit$050605479$--><span class="goog-menuitem-accel">Ctrl+Shift+Enter</span></div></div><div command="runafter" class="goog-menuitem goog-menuitem-disabled" role="menuitem" id=":24" aria-disabled="true" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Run cell and below<!--?lit$050605479$--><span class="goog-menuitem-accel">Ctrl+F10</span></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":25" style="user-select: none;"></div><div command="interrupt" class=" goog-menuitem " role="menuitem" id=":26" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Interrupt execution<!--?lit$050605479$--><span class="goog-menuitem-accel">Ctrl+M I</span></div></div><div command="restart" class=" goog-menuitem " role="menuitem" id=":27" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Restart session<!--?lit$050605479$--><span class="goog-menuitem-accel">Ctrl+M .</span></div></div><div command="restart-and-run-all" class=" goog-menuitem " role="menuitem" id=":28" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Restart session and run all<!--?lit$050605479$--></div></div><div command="powerwash-current-vm" class=" goog-menuitem " role="menuitem" id=":29" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Disconnect and delete runtime<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":2a" style="user-select: none;"></div><div command="change-runtime-type" class=" goog-menuitem " role="menuitem" id=":2b" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Change runtime type<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":2c" style="user-select: none;"></div><div command="manage-sessions" class=" goog-menuitem " role="menuitem" id=":2d" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Manage sessions<!--?lit$050605479$--></div></div><div command="open-resource-viewer" class=" goog-menuitem " role="menuitem" id=":2e" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->View resources<!--?lit$050605479$--></div></div><div command="view-runtime-logs" class=" goog-menuitem " role="menuitem" id=":2f" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->View runtime logs<!--?lit$050605479$--></div></div></div><div class="goog-menu" id="tools-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$050605479$--><div command="show-command-palette" class=" goog-menuitem " role="menuitem" id=":2h" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Command palette<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":2i" style="user-select: none;"></div><div command="preferences" class=" goog-menuitem " role="menuitem" id=":2j" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Settings<!--?lit$050605479$--></div></div><div command="shortcuts" class=" goog-menuitem " role="menuitem" id=":2k" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Keyboard shortcuts<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":2l" style="user-select: none;"></div><div command="open-differ" class=" goog-menuitem " role="menuitem" id=":2m" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Diff notebooks<!--?lit$050605479$--> <span class="screenreader-only" style="user-select: none;"><!--?lit$050605479$-->(opens in a new tab)</span></div></div></div><div class="goog-menu" id="help-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$050605479$--><div command="faq" class=" goog-menuitem " role="menuitem" id=":2o" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Frequently asked questions<!--?lit$050605479$--></div></div><div command="view-relnotes" class=" goog-menuitem " role="menuitem" id=":2p" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->View release notes<!--?lit$050605479$--></div></div><div command="snippets" class=" goog-menuitem " role="menuitem" id=":2q" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Search code snippets<!--?lit$050605479$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":2r" style="user-select: none;"></div><div command="report-bug" class=" goog-menuitem " role="menuitem" id=":2s" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Report a bug<!--?lit$050605479$--></div></div><div command="report-abuse" class=" goog-menuitem " role="menuitem" id=":2t" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Report Drive abuse<!--?lit$050605479$--></div></div><div command="send-feedback" class=" goog-menuitem " role="menuitem" id=":2u" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->Send feedback<!--?lit$050605479$--></div></div><div command="view-tos" class=" goog-menuitem " role="menuitem" id=":2v" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$050605479$-->View terms of service<!--?lit$050605479$--></div></div></div><dialog class="doc-comments-area" aria-label="Comments"><!----><div class="doc-comments-buttons">
        <md-text-button command="add-comment" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$050605479$-->
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$050605479$--><button id="button" class="button">
      <!--?lit$050605479$-->
      <span class="touch"></span>
      <!--?lit$050605479$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$050605479$-->
    
    </button>
    </template>
          <md-icon slot="icon" filled="" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>comment</md-icon>
          <!--?lit$050605479$-->Add a comment
        </md-text-button>
      </div></dialog><div class="thumbnail"></div><div class="monaco-aria-container"><div class="monaco-alert" role="alert" aria-atomic="true"></div><div class="monaco-alert" role="alert" aria-atomic="true"></div><div class="monaco-status" role="complementary" aria-live="polite" aria-atomic="true"></div><div class="monaco-status" role="complementary" aria-live="polite" aria-atomic="true"></div></div><iframe id="apiproxy40f07c85454be4011a6cad5aec86c1b736d5a5110.366784036" name="apiproxy40f07c85454be4011a6cad5aec86c1b736d5a5110.366784036" src="./Untitled21.ipynb - Colab_files/proxy.html" tabindex="-1" aria-hidden="true" style="width: 1px; height: 1px; position: absolute; top: -100px; display: none;"></iframe><div><div class="grecaptcha-badge" data-style="bottomright" style="width: 256px; height: 60px; position: fixed; visibility: hidden; display: block; transition: right 0.3s; bottom: 14px; right: -186px; box-shadow: gray 0px 0px 5px; border-radius: 2px; overflow: hidden;"><div class="grecaptcha-logo"><iframe title="reCAPTCHA" width="256" height="60" role="presentation" name="a-sua8tlmxvtzb" frameborder="0" scrolling="no" sandbox="allow-forms allow-popups allow-same-origin allow-scripts allow-top-navigation allow-modals allow-popups-to-escape-sandbox allow-storage-access-by-user-activation" src="./Untitled21.ipynb - Colab_files/anchor.html"></iframe></div><div class="grecaptcha-error"></div><textarea id="g-recaptcha-response-100000" name="g-recaptcha-response" class="g-recaptcha-response" style="width: 250px; height: 40px; border: 1px solid rgb(193, 193, 193); margin: 10px 25px; padding: 0px; resize: none; display: none;"></textarea></div><iframe style="display: none;" src="./Untitled21.ipynb - Colab_files/saved_resource(1).html"></iframe></div><iframe id="apiproxyb4ca6ba0ad853deb9ac9cda83eee963bb2f374840.3773440459" name="apiproxyb4ca6ba0ad853deb9ac9cda83eee963bb2f374840.3773440459" src="./Untitled21.ipynb - Colab_files/proxy(1).html" tabindex="-1" aria-hidden="true" style="width: 1px; height: 1px; position: absolute; top: -100px; display: none;"></iframe><iframe src="./Untitled21.ipynb - Colab_files/bscframe.html" style="display: none;"></iframe></body></html> - Colab.html…]()


---

📌 *This README file provides an overview of key findings from the dataset analysis. For more details, refer to the full dataset and code implementation in this repository.*  

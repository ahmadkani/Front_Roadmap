### **مفاهیم اصلی هر بخش:**

#### **۱. مبانی جاوا اسکریپت و تعامل با مرورگر**  
- **Execution Context** | **Hoisting** | **Closures**  
- **Prototype Chain** | **Class** 
- **DOM Optimization** | **Reflow & Repaint**  
- **Event Delegation** | **Custom Events**  
- **Event Loop** | **Microtask Queue** | **Callback Queue**  
- **Async/Await** | **Promise.all** | **Error Handling**  

#### **۲. ذخیره‌سازی سمت کاربر و شبکه**  
- **IndexedDB** | **Object Store** | **Transactions**  
- **Schema Design** | **Versioning** | **Cursor Queries**  
- **Fetch API** | **Streaming Data** | **AbortController**  
- **Offline-First** | **Conflict Resolution**  

#### **۳. ابزارهای پیشرفته و امنیت**  
- **Git Internals** | **Plumbing Commands** | **Blob/Tree/Commit**  
- **Web Crypto API** | **AES-GCM** | **Hashing**  
- **OpenPGP.js** | **Asymmetric Encryption** | **Digital Signatures**  

#### **۴. معماری فرانت‌اند مدرن**  
- **Web Components** | **Shadow DOM** | **Custom Elements**  
- **State Management** | **Event-Driven Architecture**  
- **Sandboxing** | **postMessage** | **Dynamic Code Execution**  

---
### پروژه‌ها

**پروژه اول: ویرایشگر اسناد رمزنگاری شده با ورژن‌بندی سمت کاربر**
این پروژه یک ویرایشگر متن شبیه به Notion یا Google Docs است که تمام عملیات آن در مرورگر کاربر انجام می‌شود.
*   مهارت آموزان باید سیستم ورژن‌بندی (Versioning) این ویرایشگر را با الهام از مدل داده Git (مفاهیم blob, tree, commit) در داخل IndexedDB پیاده‌سازی کنند. علاوه بر این، کاربر باید بتواند تمام دیتابیس خود را با یک کلید GPG که در اختیار خودش است، به صورت یک فایل رمزنگاری شده خروجی بگیرد.
	* برای این پروژه از کتابخانه ی isomorphic git استفاده کنید.

**پروژه دوم: وایت‌بورد تعاملی Peer-to-Peer (P2P)**
یک وایت‌بورد آنلاین که چندین کاربر می‌توانند به صورت همزمان روی آن طراحی کنند.
*   ارتباط بین کاربران باید مستقیماً و بدون سرور مرکزی، از طریق تکنولوژی WebRTC (Peer-to-Peer) برقرار شود. مدیریت حالت (State) همزمان بین چندین کاربر، حل تداخل‌ها (Conflict Resolution) و اطمینان از اینکه همه کاربران یک نسخه یکسان از وایت‌بورد را می‌بینند، چالش اصلی این پروژه است. این پروژه نیازمند تسلط بر تمام مفاهیم دوره از جمله Web Components برای UI، IndexedDB برای ذخیره‌سازی محلی و درک عمیق از مفاهیم شبکه غیرمتمرکز است.

<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>لوحة إدارة المنيو</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root { --bg:#f5f6fa; --card:#fff; --accent:#d4af37; --grad:linear-gradient(135deg,#f39c12,#d4af37); --text:#2f3640; --muted:#718093; --border:rgba(0,0,0,.08); --ok:#27ae60; --bad:#ff4757; --shadow:0 8px 24px rgba(0,0,0,.08); }
    * { box-sizing:border-box; margin:0; padding:0; font-family:'Cairo',sans-serif; -webkit-tap-highlight-color:transparent; }
    body { background:var(--bg); color:var(--text); padding:12px 12px 100px; }
    .hidden { display:none !important; }
    .wrap { max-width:800px; margin:0 auto; }
    .card { background:var(--card); border:1px solid var(--border); border-radius:16px; padding:14px; margin-bottom:12px; box-shadow:var(--shadow); }
    .card h2 { font-size:.95rem; font-weight:700; margin-bottom:12px; padding-bottom:8px; border-bottom:1px solid var(--border); display:flex; justify-content:space-between; align-items:center; gap:6px; flex-wrap:wrap; }
    .login { max-width:400px; margin:12vh auto 0; text-align:center; }
    .login h1 { color:var(--accent); font-size:1.2rem; font-weight:800; margin-bottom:16px; }
    .field { margin-bottom:10px; text-align:right; }
    .field label { display:block; font-size:.8rem; color:var(--muted); font-weight:600; margin-bottom:4px; }
    .field input, .field select, .field textarea { width:100%; padding:12px; border-radius:12px; border:1px solid var(--border); background:#fdfdfd; font-size:16px; outline:none; color:var(--text); }
    .field input:focus, .field select:focus, .field textarea:focus { border-color:var(--accent); box-shadow:0 0 0 3px rgba(212,175,55,.15); }
    .grid { display:grid; grid-template-columns:1fr; gap:10px; }
    @media(min-width:550px){ .grid { grid-template-columns:1fr 1fr; } .span2 { grid-column:1/-1; } }
    .btn { width:100%; padding:13px; background:var(--grad); border:none; border-radius:12px; color:#fff; font-weight:700; font-size:.95rem; cursor:pointer; }
    .btn:active { transform:scale(.98); }
    .btn.ok { background:var(--ok); } .btn.bad { background:var(--bad); } .btn.ghost { background:#fff; color:var(--text); border:1px solid var(--border); }
    .btn.sm { width:auto; padding:8px 12px; font-size:.75rem; border-radius:10px; }
    .top { display:flex; justify-content:space-between; align-items:center; gap:10px; flex-wrap:wrap; }
    .top h1 { color:var(--accent); font-size:1rem; font-weight:800; }
    .tabs { display:flex; gap:6px; overflow-x:auto; margin-bottom:12px; padding-bottom:4px; scrollbar-width:none; }
    .tabs::-webkit-scrollbar { display:none; }
    .tab { flex:0 0 auto; padding:10px 14px; background:var(--card); border:1px solid var(--border); border-radius:12px; color:var(--muted); font-weight:700; font-size:.8rem; cursor:pointer; }
    .tab.active { background:var(--grad); color:#fff; border-color:transparent; }
    .row { display:flex; flex-direction:column; gap:8px; padding:10px; border:1px solid var(--border); background:#fafbfc; margin-bottom:8px; border-radius:12px; }
    @media(min-width:480px){ .row { flex-direction:row; justify-content:space-between; align-items:center; } }
    .row .info small { display:block; font-size:.75rem; color:var(--muted); }
    .row .acts { display:flex; gap:6px; flex-wrap:wrap; }
    .badge { padding:4px 10px; border-radius:20px; font-size:.7rem; font-weight:700; border:1px solid; }
    .badge.ok { background:rgba(39,174,96,.12); color:var(--ok); border-color:var(--ok); }
    .badge.bad { background:rgba(255,71,87,.12); color:var(--bad); border-color:var(--bad); }
    .toggle { padding:10px 12px; border-radius:10px; font-weight:700; cursor:pointer; font-size:.75rem; border:1px solid; }
    .toggle.ok { background:rgba(39,174,96,.12); color:var(--ok); border-color:var(--ok); }
    .toggle.bad { background:rgba(255,71,87,.12); color:var(--bad); border-color:var(--bad); }
    .err { color:var(--bad); font-size:.8rem; margin-top:10px; }
    .empty { text-align:center; color:var(--muted); padding:15px; font-size:.85rem; }
    .toast { position:fixed; bottom:20px; left:50%; transform:translateX(-50%); background:#2f3640; color:#fff; padding:10px 18px; border-radius:12px; font-size:.85rem; z-index:99; opacity:0; transition:.3s; pointer-events:none; }
    .toast.show { opacity:1; }
    .check { display:flex; align-items:center; gap:8px; font-size:.85rem; font-weight:600; padding-top:6px; }
    .check input { width:20px; height:20px; }
  </style>
</head>
<body>
<div class="wrap">

  <!-- تسجيل الدخول -->
  <div id="loginView" class="card login">
    <h1>تسجيل الدخول</h1>
    <div class="field"><label>الإيميل</label><input type="email" id="email" autocomplete="username" dir="ltr"></div>
    <div class="field"><label>كلمة المرور</label><input type="password" id="password" autocomplete="current-password" dir="ltr"></div>
    <button class="btn" id="loginBtn">دخول</button>
    <p class="err hidden" id="loginErr"></p>
  </div>

  <!-- اختيار المنيو (للسوبر أدمن فقط) -->
  <div id="pickerView" class="hidden">
    <div class="card">
      <div class="top"><h1>اختيار منيو</h1><button class="btn ghost sm" data-logout>تسجيل خروج</button></div>
    </div>
    <div class="card">
      <h2>المنيوات الموجودة</h2>
      <div id="menuList"></div>
    </div>
    <div class="card">
      <h2>إنشاء منيو جديد</h2>
      <div class="grid">
        <div class="field"><label>معرف المنيو بالإنجليزي (حروف صغيرة وأرقام و - فقط)</label><input id="newMenuId" dir="ltr" placeholder="restaurant1"></div>
        <div class="field"><label>اسم المطعم</label><input id="newMenuName"></div>
      </div>
      <button class="btn ok" id="createMenuBtn">إنشاء ➕</button>
    </div>
  </div>

  <!-- لوحة التحكم -->
  <div id="dashView" class="hidden">
    <div class="card top">
      <h1>منيو: <span id="menuTitle" dir="ltr"></span></h1>
      <div class="acts" style="display:flex;gap:6px">
        <button class="btn ghost sm hidden" id="backBtn">رجوع للقائمة</button>
        <button class="btn ghost sm" data-logout>خروج</button>
      </div>
    </div>

    <div class="tabs" id="tabs">
      <button class="tab active" data-tab="general">الواجهة</button>
      <button class="tab" data-tab="categories">الأقسام</button>
      <button class="tab" data-tab="meals">الوجبات</button>
      <button class="tab" data-tab="status">حالة الوجبات</button>
    </div>

    <!-- الواجهة -->
    <section id="tab-general">
      <div class="card" id="subCard">
        <h2><span>الاشتراك</span><span class="badge" id="subBadge"></span></h2>
        <div class="grid">
          <div class="field"><label>تاريخ انتهاء الاشتراك</label><input type="date" id="expiresAt"></div>
          <div class="field"><label>الحالة</label>
            <select id="subStatus"><option value="active">نشط</option><option value="expired">منتهي / موقوف</option></select>
          </div>
        </div>
        <button class="btn" id="saveSubBtn">حفظ الاشتراك</button>
      </div>
      <div class="card">
        <h2>معلومات الواجهة</h2>
        <div class="grid">
          <div class="field"><label>اسم المطعم</label><input id="lName"></div>
          <div class="field"><label>وصف ترحيبي</label><input id="lDesc"></div>
          <div class="field span2"><label>رابط الشعار</label><input id="lLogo" dir="ltr" placeholder="https://..."></div>
          <div class="field"><label>فيسبوك</label><input id="lFb" dir="ltr" placeholder="https://facebook.com/..."></div>
          <div class="field"><label>انستغرام</label><input id="lInsta" dir="ltr" placeholder="https://instagram.com/..."></div>
          <div class="field span2"><label>واتساب / تليجرام</label><input id="lOther" dir="ltr" placeholder="https://t.me/..."></div>
        </div>
        <button class="btn" id="saveLandingBtn">حفظ 💾</button>
      </div>
    </section>

    <!-- الأقسام -->
    <section id="tab-categories" class="hidden">
      <div class="card">
        <h2>إضافة قسم</h2>
        <div class="grid">
          <div class="field"><label>معرف القسم (إنجليزي، مثل burgers)</label><input id="cId" dir="ltr"></div>
          <div class="field"><label>الاسم بالعربي</label><input id="cAr"></div>
          <div class="field span2"><label>الاسم بالإنجليزي</label><input id="cEn" dir="ltr"></div>
        </div>
        <button class="btn ok" id="addCatBtn">إضافة ➕</button>
      </div>
      <div class="card"><h2>الأقسام الحالية</h2><div id="catList"></div></div>
    </section>

    <!-- الوجبات -->
    <section id="tab-meals" class="hidden">
      <div class="card">
        <h2><span id="mealFormTitle">إضافة وجبة</span></h2>
        <div class="grid">
          <div class="field"><label>الاسم (عربي)</label><input id="mTitleAr"></div>
          <div class="field"><label>الاسم (إنجليزي)</label><input id="mTitleEn" dir="ltr"></div>
          <div class="field"><label>الوصف (عربي)</label><input id="mDescAr"></div>
          <div class="field"><label>الوصف (إنجليزي)</label><input id="mDescEn" dir="ltr"></div>
          <div class="field"><label>السعر بالدينار (أرقام فقط)</label><input id="mPrice" type="number" inputmode="numeric" min="0" step="250" dir="ltr"></div>
          <div class="field"><label>القسم</label><select id="mCat"></select></div>
          <div class="field span2"><label>رابط الصورة</label><input id="mImg" dir="ltr" placeholder="https://..."></div>
          <label class="check span2"><input type="checkbox" id="mFeatured"> وجبة مميزة ⭐</label>
        </div>
        <div style="display:flex;gap:8px;margin-top:12px">
          <button class="btn ok" id="saveMealBtn">حفظ الوجبة 🚀</button>
          <button class="btn ghost hidden" id="cancelEditBtn">إلغاء التعديل</button>
        </div>
      </div>
      <div class="card"><h2>الوجبات</h2><div id="mealList"></div></div>
    </section>

    <!-- حالة الوجبات -->
    <section id="tab-status" class="hidden">
      <div class="card"><h2>متوفر / غير متوفر (يتحدث مباشرة)</h2><div id="statusList"></div></div>
    </section>
  </div>
</div>
<div class="toast" id="toast"></div>

<script type="module">
  import { initializeApp } from "https://www.gstatic.com/firebasejs/10.14.1/firebase-app.js";
  import { getAuth, signInWithEmailAndPassword, signOut, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/10.14.1/firebase-auth.js";
  import { getDatabase, ref, get, set, update, remove, onValue } from "https://www.gstatic.com/firebasejs/10.14.1/firebase-database.js";
  import { firebaseConfig } from "./firebase-config.js";

  const app = initializeApp(firebaseConfig);
  const auth = getAuth(app);
  const db = getDatabase(app);

  const $ = id => document.getElementById(id);
  const show = (id, on = true) => $(id).classList.toggle('hidden', !on);

  // بناء عناصر بشكل آمن (بدون innerHTML) لمنع ثغرات XSS
  function el(tag, props = {}, ...kids) {
    const n = document.createElement(tag);
    for (const [k, v] of Object.entries(props)) {
      if (k === 'class') n.className = v;
      else if (k.startsWith('on')) n.addEventListener(k.slice(2), v);
      else n.setAttribute(k, v);
    }
    kids.flat().forEach(c => n.append(c instanceof Node ? c : document.createTextNode(c)));
    return n;
  }
  let toastTimer;
  function toast(msg) {
    const t = $('toast'); t.textContent = msg; t.classList.add('show');
    clearTimeout(toastTimer); toastTimer = setTimeout(() => t.classList.remove('show'), 2200);
  }
  const fmtPrice = n => (Number(n) || 0).toLocaleString('en-US') + ' د.ع';
  const safeUrl = u => /^https?:\/\//i.test(u) ? u : '';
  const toArr = obj => Object.entries(obj || {}).map(([id, v]) => ({ id, ...v }));

  let profile = null;   // {role, menuId}
  let menuId = null;
  let menu = {};        // نسخة حية من menus/{menuId}
  let unsub = null;
  let editingMealId = null;
  const isAdmin = () => profile?.role === 'admin';

  /* ---------- الدخول ---------- */
  $('loginBtn').onclick = async () => {
    const err = $('loginErr'); err.classList.add('hidden');
    try {
      await signInWithEmailAndPassword(auth, $('email').value.trim(), $('password').value);
    } catch (e) {
      err.textContent = 'الإيميل أو كلمة المرور غير صحيحة.'; err.classList.remove('hidden');
    }
  };
  $('password').addEventListener('keydown', e => { if (e.key === 'Enter') $('loginBtn').click(); });
  document.querySelectorAll('[data-logout]').forEach(b => b.onclick = () => signOut(auth));

  onAuthStateChanged(auth, async user => {
    if (unsub) { unsub(); unsub = null; }
    show('loginView', !user); show('pickerView', false); show('dashView', false);
    if (!user) { profile = null; return; }
    try {
      const snap = await get(ref(db, `users/${user.uid}`));
      profile = snap.val();
    } catch { profile = null; }
    if (!profile || !['admin', 'owner'].includes(profile.role)) {
      await signOut(auth);
      const err = $('loginErr');
      err.textContent = profile?.role === 'staff' ? 'هذا الحساب للستاف، استعمل صفحة staff.html.' : 'هذا الحساب غير مفعّل. راجع المشرف.';
      err.classList.remove('hidden'); return;
    }
    if (isAdmin()) await openPicker(); else openMenu(profile.menuId);
  });

  /* ---------- اختيار المنيو (سوبر أدمن) ---------- */
  async function openPicker() {
    show('pickerView'); show('dashView', false);
    const list = $('menuList'); list.replaceChildren();
    const snap = await get(ref(db, 'menuIndex'));
    const items = toArr(snap.val());
    if (!items.length) list.append(el('p', { class: 'empty' }, 'لا توجد منيوات بعد.'));
    items.forEach(m => list.append(
      el('div', { class: 'row' },
        el('div', { class: 'info' }, el('strong', {}, m.name || m.id), el('small', { dir: 'ltr' }, m.id)),
        el('button', { class: 'btn sm', onclick: () => openMenu(m.id) }, 'فتح'))
    ));
  }
  $('createMenuBtn').onclick = async () => {
    const id = $('newMenuId').value.trim().toLowerCase();
    const name = $('newMenuName').value.trim();
    if (!/^[a-z0-9_-]{2,40}$/.test(id) || !name) return toast('المعرف: حروف إنجليزية صغيرة وأرقام فقط، والاسم مطلوب');
    const exists = await get(ref(db, `menuIndex/${id}`));
    if (exists.exists()) return toast('هذا المعرف مستخدم');
    await update(ref(db), {
      [`menus/${id}/status`]: 'active',
      [`menus/${id}/landing/name`]: name,
      [`menuIndex/${id}`]: { name }
    });
    $('newMenuId').value = ''; $('newMenuName').value = '';
    toast('تم إنشاء المنيو'); openPicker();
  };
  $('backBtn').onclick = () => { if (unsub) unsub(); unsub = null; openPicker(); };

  /* ---------- لوحة المنيو ---------- */
  function openMenu(id) {
    menuId = id;
    show('pickerView', false); show('dashView');
    show('backBtn', isAdmin()); show('subCard', isAdmin());
    $('menuTitle').textContent = id;
    switchTab('general');
    if (unsub) unsub();
    unsub = onValue(ref(db, `menus/${id}`), snap => {
      menu = snap.val() || {};
      renderAll();
    }, () => toast('تعذر تحميل المنيو'));
  }

  function switchTab(name) {
    document.querySelectorAll('.tab').forEach(t => t.classList.toggle('active', t.dataset.tab === name));
    ['general', 'categories', 'meals', 'status'].forEach(n => show('tab-' + n, n === name));
  }
  document.querySelectorAll('.tab').forEach(t => t.onclick = () => switchTab(t.dataset.tab));

  const cats = () => toArr(menu.categories).sort((a, b) => (a.order ?? 0) - (b.order ?? 0));
  const meals = () => toArr(menu.meals);
  const catName = id => (menu.categories?.[id]?.ar) || id;

  function renderAll() { renderGeneral(); renderCats(); renderMealForm(); renderMeals(); renderStatus(); }

  function renderGeneral() {
    const st = menu.status === 'expired' ? 'expired' : 'active';
    const b = $('subBadge'); b.className = 'badge ' + (st === 'active' ? 'ok' : 'bad');
    b.textContent = st === 'active' ? 'نشط' : 'منتهي';
    $('subStatus').value = st; $('expiresAt').value = menu.expiresAt || '';
    // لا نكتب فوق الحقول إذا المستخدم يكتب فيها حالياً
    if (document.activeElement?.closest('#tab-general .card:not(#subCard)')) return;
    const l = menu.landing || {};
    $('lName').value = l.name || ''; $('lDesc').value = l.desc || ''; $('lLogo').value = l.logo || '';
    const soc = p => (l.socials || []).find(s => s.platform === p)?.url || '';
    $('lFb').value = soc('Facebook'); $('lInsta').value = soc('Instagram'); $('lOther').value = soc('Telegram');
  }

  $('saveSubBtn').onclick = async () => {
    await update(ref(db, `menus/${menuId}`), { status: $('subStatus').value, expiresAt: $('expiresAt').value || null });
    toast('تم حفظ الاشتراك');
  };
  $('saveLandingBtn').onclick = async () => {
    const socials = [];
    const add = (platform, icon, v) => { const u = safeUrl(v.trim()); if (u) socials.push({ platform, icon, url: u }); };
    add('Facebook', 'fab fa-facebook-f', $('lFb').value);
    add('Instagram', 'fab fa-instagram', $('lInsta').value);
    add('Telegram', 'fab fa-telegram-plane', $('lOther').value);
    const landing = { name: $('lName').value.trim(), desc: $('lDesc').value.trim(), logo: safeUrl($('lLogo').value.trim()), socials };
    const ups = { [`menus/${menuId}/landing`]: landing };
    if (isAdmin()) ups[`menuIndex/${menuId}/name`] = landing.name || menuId;
    await update(ref(db), ups);
    toast('تم الحفظ');
  };

  /* ---------- الأقسام ---------- */
  function renderCats() {
    const list = $('catList'); list.replaceChildren();
    const arr = cats();
    if (!arr.length) list.append(el('p', { class: 'empty' }, 'لا توجد أقسام.'));
    arr.forEach((c, i) => list.append(
      el('div', { class: 'row' },
        el('div', { class: 'info' }, el('strong', {}, c.ar), el('small', { dir: 'ltr' }, `${c.en || ''} (${c.id})`)),
        el('div', { class: 'acts' },
          el('button', { class: 'btn ghost sm', onclick: () => moveCat(i, -1) }, '▲'),
          el('button', { class: 'btn ghost sm', onclick: () => moveCat(i, 1) }, '▼'),
          el('button', { class: 'btn bad sm', onclick: () => deleteCat(c.id) }, 'حذف')))
    ));
    // قائمة الأقسام بنموذج الوجبة
    const sel = $('mCat'); const cur = sel.value; sel.replaceChildren();
    arr.forEach(c => sel.append(el('option', { value: c.id }, c.ar)));
    if (cur && menu.categories?.[cur]) sel.value = cur;
  }
  $('addCatBtn').onclick = async () => {
    const id = $('cId').value.trim().toLowerCase(), ar = $('cAr').value.trim(), en = $('cEn').value.trim();
    if (!/^[a-z0-9_-]{1,40}$/.test(id) || !ar) return toast('المعرف إنجليزي (حروف وأرقام) والاسم العربي مطلوب');
    if (menu.categories?.[id]) return toast('هذا المعرف موجود');
    await set(ref(db, `menus/${menuId}/categories/${id}`), { ar, en: en || ar, order: cats().length });
    ['cId', 'cAr', 'cEn'].forEach(i => $(i).value = '');
    toast('تمت إضافة القسم');
  };
  async function moveCat(i, d) {
    const arr = cats(), j = i + d;
    if (j < 0 || j >= arr.length) return;
    [arr[i], arr[j]] = [arr[j], arr[i]];
    const ups = {}; arr.forEach((c, idx) => ups[`menus/${menuId}/categories/${c.id}/order`] = idx);
    await update(ref(db), ups);
  }
  async function deleteCat(id) {
    if (meals().some(m => m.category === id)) return toast('لا يمكن الحذف: فيه وجبات بهذا القسم');
    if (!confirm('حذف هذا القسم؟')) return;
    await remove(ref(db, `menus/${menuId}/categories/${id}`));
  }

  /* ---------- الوجبات (إضافة + تعديل + حذف) ---------- */
  function renderMealForm() {
    $('mealFormTitle').textContent = editingMealId ? 'تعديل وجبة' : 'إضافة وجبة';
    show('cancelEditBtn', !!editingMealId);
  }
  function clearMealForm() {
    editingMealId = null;
    ['mTitleAr', 'mTitleEn', 'mDescAr', 'mDescEn', 'mPrice', 'mImg'].forEach(i => $(i).value = '');
    $('mFeatured').checked = false; renderMealForm();
  }
  $('cancelEditBtn').onclick = clearMealForm;

  function startEdit(m) {
    editingMealId = m.id;
    $('mTitleAr').value = m.title_ar || ''; $('mTitleEn').value = m.title_en || '';
    $('mDescAr').value = m.desc_ar || ''; $('mDescEn').value = m.desc_en || '';
    $('mPrice').value = m.price ?? ''; $('mImg').value = m.img || '';
    $('mCat').value = m.category; $('mFeatured').checked = !!m.featured;
    renderMealForm(); switchTab('meals'); window.scrollTo({ top: 0, behavior: 'smooth' });
  }

  $('saveMealBtn').onclick = async () => {
    const titleAr = $('mTitleAr').value.trim(), category = $('mCat').value;
    const price = Number($('mPrice').value);
    if (!titleAr || !category) return toast('اسم الوجبة والقسم مطلوبين');
    if (!(price >= 0) || $('mPrice').value === '') return toast('اكتب السعر بالأرقام');
    const id = editingMealId || ('meal_' + Date.now());
    const old = menu.meals?.[id] || {};
    const meal = {
      title_ar: titleAr, title_en: $('mTitleEn').value.trim() || titleAr,
      desc_ar: $('mDescAr').value.trim(), desc_en: $('mDescEn').value.trim() || $('mDescAr').value.trim(),
      price, category, featured: $('mFeatured').checked,
      img: safeUrl($('mImg').value.trim()) || 'https://images.unsplash.com/photo-1546069901-ba9599a7e63c?w=500',
      createdAt: old.createdAt || Date.now()
    };
    // حقول قديمة تحتاجها صفحة المنيو الحالية
    meal.title = meal.title_ar; meal.desc = meal.desc_ar;
    await set(ref(db, `menus/${menuId}/meals/${id}`), meal);
    toast(editingMealId ? 'تم تعديل الوجبة' : 'تمت إضافة الوجبة');
    clearMealForm();
  };

  function renderMeals() {
    const list = $('mealList'); list.replaceChildren();
    const arr = meals().sort((a, b) => (a.createdAt || 0) - (b.createdAt || 0));
    if (!arr.length) return list.append(el('p', { class: 'empty' }, 'لا توجد وجبات.'));
    arr.forEach(m => list.append(
      el('div', { class: 'row' },
        el('div', { class: 'info' },
          el('strong', {}, (m.featured ? '⭐ ' : '') + (m.title_ar || m.title)),
          el('small', {}, `${catName(m.category)} | ${fmtPrice(m.price)}`)),
        el('div', { class: 'acts' },
          el('button', { class: 'btn ghost sm', onclick: () => startEdit(m) }, 'تعديل'),
          el('button', { class: 'btn bad sm', onclick: async () => {
            if (!confirm('حذف الوجبة؟')) return;
            await update(ref(db), { [`menus/${menuId}/meals/${m.id}`]: null, [`menus/${menuId}/soldout/${m.id}`]: null });
          } }, 'حذف')))
    ));
  }

  /* ---------- حالة الوجبات ---------- */
  function renderStatus() {
    const list = $('statusList'); list.replaceChildren();
    const arr = meals();
    if (!arr.length) return list.append(el('p', { class: 'empty' }, 'لا توجد وجبات.'));
    arr.forEach(m => {
      const out = menu.soldout?.[m.id] === true;
      list.append(el('div', { class: 'row' },
        el('div', { class: 'info' }, el('strong', {}, m.title_ar || m.title), el('small', {}, catName(m.category))),
        el('button', { class: 'toggle ' + (out ? 'bad' : 'ok'),
          onclick: () => set(ref(db, `menus/${menuId}/soldout/${m.id}`), out ? null : true) },
          out ? 'غير متوفر 🔴' : 'متوفر 🟢')));
    });
  }
</script>
</body>
</html>

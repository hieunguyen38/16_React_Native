# 📱 TỰ HỌC REACT NATIVE (BASIC) TỪ SỐ 0

> Tài liệu tổng hợp khóa học **Tự Học React Native — Làm App Mobile Android/iOS Cho Người Mới Bắt Đầu Từ Số 0** từ kênh **Hỏi Dân IT với Eric** (YouTube).
> Bổ sung thêm kiến thức React Native chuẩn, giải thích chi tiết các Core Component, Styling (Flexbox), Navigation và bổ sung **góc nhìn dành cho dân Embedded** 🔧.

📚 Tài liệu tổng hợp từ slide PDF khóa học (24 Bước) + playlist **36 videos** trên YouTube (cập nhật 15/10/2025), kèm version thư viện chính xác để code theo không lỗi.

⚠️ **React Native** là framework do **Facebook (Meta)** phát triển — viết **một lần bằng JavaScript**, chạy được trên **cả Android & iOS** (và Web). Bắt buộc phải biết nếu muốn làm **Mobile Developer** bằng JS.

> 🔧 **Dành cho dân Embedded**: Nếu bạn đã quen với C/C++ trên ESP32/STM32, hãy để ý các callout **📌 Góc nhìn Embedded** rải khắp tài liệu — mình map từng khái niệm React Native sang khái niệm nhúng quen thuộc (state ↔ biến global, component lifecycle ↔ `setup()`/`loop()`, event ↔ interrupt...) để bạn vào nghề nhanh hơn.

---

## 📑 MỤC LỤC TỔNG QUAN

```
==============================================================
| CHAPTER   | NỘI DUNG                                       |
==============================================================
| CHAPTER 1 | GIỚI THIỆU & MÔI TRƯỜNG (Bước 1-3)             |
| CHAPTER 2 | CORE COMPONENTS & STYLING (Bước 4-8)           |
| CHAPTER 3 | DỰ ÁN TODO LIST (Bước 9-13)                    |
| CHAPTER 4 | FONTS & NAVIGATION (Bước 14-20)                |
| CHAPTER 5 | IMAGES, MODAL & HOÀN THIỆN (Bước 21-24)        |
| BONUS     | EMBEDDED VIEW + CHEAT SHEET + ROADMAP          |
==============================================================
```

### 🔖 Chi tiết các bài học

<details>
<summary><b>Chapter 1: Giới thiệu & Môi trường</b></summary>

- [#1. Giới Thiệu React Native & Expo](#1-giới-thiệu-react-native--expo)
- [#2. Cách Đọc & Tự Học React Native](#2-cách-đọc--tự-học-react-native)
- [#3. Setup Môi Trường Khóa Học](#3-setup-môi-trường-khóa-học)
</details>

<details>
<summary><b>Chapter 2: Core Components & Styling</b></summary>

- [#4. View, Text & Styles](#4-view-text--styles)
- [#5. Sử Dụng State & Button](#5-sử-dụng-state--button)
- [#6. Text Inputs](#6-text-inputs)
- [#7. Sử Dụng Array (Render List + ScrollView)](#7-sử-dụng-array-render-list--scrollview)
- [#8. Flat List](#8-flat-list)
</details>

<details>
<summary><b>Chapter 3: Dự Án Todo List</b></summary>

- [#9. Todo List (Part 1)](#9-todo-list-part-1)
- [#10. Todo List (Part 2) — Pressable](#10-todo-list-part-2--pressable)
- [#11. Feedback với Alert & Keyboard](#11-feedback-với-alert--keyboard)
- [#12. Flex Box (Basic)](#12-flex-box-basic)
- [#13. Sử Dụng Icons (Hoàn thiện Todo)](#13-sử-dụng-icons-hoàn-thiện-todo)
</details>

<details>
<summary><b>Chapter 4: Fonts & Navigation</b></summary>

- [#14. Sử Dụng Fonts](#14-sử-dụng-fonts)
- [#15. Giới Thiệu Navigation](#15-giới-thiệu-navigation)
- [#16. Hello React Navigation](#16-hello-react-navigation)
- [#17. Moving Between Screens](#17-moving-between-screens)
- [#18. Passing Parameters To Routes](#18-passing-parameters-to-routes)
- [#19. Drawer Navigator](#19-drawer-navigator)
- [#20. Custom Header](#20-custom-header)
</details>

<details>
<summary><b>Chapter 5: Images, Modal & Hoàn Thiện</b></summary>

- [#21. Sử Dụng Images](#21-sử-dụng-images)
- [#22. Sử Dụng Modal & Form](#22-sử-dụng-modal--form)
- [#23. Hoàn Thiện Dự Án](#23-hoàn-thiện-dự-án)
- [#24. Tổng Kết](#24-tổng-kết)
</details>

<details>
<summary><b>Bonus: Embedded View + Cheat Sheet + Roadmap</b></summary>

- [#B1. React Native cho dân Embedded (Bảng so sánh)](#b1-react-native-cho-dân-embedded-bảng-so-sánh)
- [#B2. Core Components Cheat Sheet](#b2-core-components-cheat-sheet)
- [#B3. Styling & Flexbox Cheat Sheet](#b3-styling--flexbox-cheat-sheet)
- [#B4. Navigation Cheat Sheet](#b4-navigation-cheat-sheet)
- [#B5. Expo & Lệnh Thường Dùng](#b5-expo--lệnh-thường-dùng)
- [#B6. Cấu Trúc Thư Mục & Roadmap Học Tiếp](#b6-cấu-trúc-thư-mục--roadmap-học-tiếp)
</details>

---

# 📖 GIỚI THIỆU

## Về tác giả (Hỏi Dân IT)

| Kênh | Link |
|------|------|
| 🌐 Website | https://hoidanit.vn/ |
| 📺 YouTube | https://www.youtube.com/@hoidanit |
| 🎵 TikTok | https://www.tiktok.com/@hoidanit |
| 👥 Fanpage | https://www.facebook.com/askITwithERIC/ |
| 🎓 Udemy | https://www.udemy.com/user/eric-7039/ |

## ⚠️ Kiến thức yêu cầu TRƯỚC khi học

> Khóa này **KHÔNG dạy lại từ đầu** JavaScript & React. Bạn **bắt buộc** cần:

```
┌─────────────────────────────────────────────────────┐
│ 1. JavaScript ES6 (cú pháp, arrow fn, map/filter,    │
│    spread, destructuring, async/await...)            │
├─────────────────────────────────────────────────────┤
│ 2. React.js (làm Web): Component, JSX, State, Props, │
│    Hook (useState, useEffect)                        │
└─────────────────────────────────────────────────────┘
```

> 💡 Nếu bạn xuất phát từ **Embedded (C/C++)** mà chưa biết JS/React: hãy học React.js (làm web) trước. React Native dùng **chính xác** cú pháp & tư duy của React.js, chỉ thay HTML tags (`<div>`, `<p>`) bằng Native Components (`<View>`, `<Text>`).

## Phiên bản & nguyên tắc code theo video

| Mục | Yêu cầu |
|-----|---------|
| **React Native** | `v0.74` |
| **Node.js** | **bắt buộc** `v20.14.0` → [tải tại đây](https://nodejs.org/download/release/v20.14.0/) |
| **Tài liệu chính** | https://reactnative.dev/docs/getting-started |
| **Câu lệnh cài thư viện** | Gõ **đúng version** như trong video để hạn chế tối đa lỗi |
| **Source code** | Clone từ Gitlab — nhánh `starter` (code theo video), nhánh `master` (code final) |

> ⚠️ **Máy yếu (< 8GB RAM)** hoặc chạy Android Studio bị giật/lag → dùng app **Expo Go** trên điện thoại thật để test (nhẹ hơn nhiều).

---

# CHAPTER 1: GIỚI THIỆU & MÔI TRƯỜNG

> Hiểu bức tranh tổng quan trước khi code — tránh bị hổng kiến thức.

## #1. Giới Thiệu React Native & Expo

### 1. Phân biệt React / React.js / React Native

> Đây là 3 khái niệm dễ nhầm nhất với người mới.

| Tên | Bản chất | Dùng để |
|-----|----------|---------|
| **React** | **Thư viện lõi** (core) — định nghĩa Component, State, Props, Virtual DOM | Nền tảng chung, không gắn với nền tảng cụ thể |
| **React.js** (React DOM) | React + thư viện render ra **HTML DOM** | Làm **Website** (chạy trên browser) |
| **React Native** | React + thư viện render ra **Native UI** (Android/iOS) | Làm **App Mobile** |

```
                    ┌──────────────┐
                    │    REACT     │  ◄── lõi: Component, State, Props
                    │  (core lib)  │
                    └──────┬───────┘
              ┌────────────┴────────────┐
              ▼                         ▼
      ┌───────────────┐         ┌───────────────┐
      │   React DOM   │         │ React Native  │
      │  → HTML/CSS   │         │ → UIView (iOS) │
      │  (Website)    │         │ → View (Android)│
      └───────────────┘         └───────────────┘
```

### 2. "Learn once, write anywhere"

> Triết lý của React Native: **học một lần** (tư duy React) → **viết ở bất cứ đâu** (web, iOS, Android).
>
> ⚠️ Chú ý: KHÔNG phải "write once, run anywhere". Bạn vẫn cần tinh chỉnh đôi chút cho từng nền tảng — nhưng **90% logic & kiến thức dùng chung**.

### 3. Tại sao cần Expo Framework?

> **Expo** = bộ công cụ (framework + nền tảng) bọc quanh React Native, giúp **dễ bắt đầu** mà không cần cấu hình native phức tạp.

| Không có Expo (React Native "trần") | Có Expo |
|-------------------------------------|---------|
| Phải cài Android Studio / Xcode mới chạy được | Quét QR bằng app **Expo Go** → chạy ngay trên điện thoại thật |
| Cấu hình native (Java/Kotlin/Swift) thủ công | Expo lo phần native, bạn chỉ viết JS |
| Build lâu, nặng máy | Hot reload nhanh, nhẹ máy |

> 💡 Khóa học dùng Expo để người mới (và máy yếu) bắt đầu nhanh nhất.

> 📌 **Góc nhìn Embedded**: Expo giống như dùng **Arduino IDE + core board** thay vì viết thẳng register/HAL trên STM32. Arduino bọc lại phần phức tạp (clock, GPIO config) cho bạn viết `digitalWrite()` đơn giản — Expo bọc phần native cho bạn viết JS đơn giản. Khi cần "đào sâu xuống native module" thì mới `expo prebuild`/eject (giống lúc bạn bỏ Arduino core để viết bare-metal).

---

## #2. Cách Đọc & Tự Học React Native

> Mục tiêu: biết **cách tự đọc tài liệu** → không phụ thuộc video, không bị hổng kiến thức.

### 1. Tài liệu gốc

📚 https://reactnative.dev/docs/getting-started (version dùng trong khóa: **v0.74**)

### 2. Tư duy đọc docs

```
┌─────────────────────────────────────────────────────┐
│ B1. Đọc "The Basics" → Core Components, JSX, State   │
│ B2. Tra "Components" → từng component (View, Text...) │
│ B3. Tra "APIs" → Alert, Dimensions, Keyboard...      │
│ B4. Khi cần làm gì → search "react native <việc cần>"│
└─────────────────────────────────────────────────────┘
```

> 💡 Mỗi component trong docs đều có: **mô tả → ví dụ code chạy được → bảng Props**. Học cách đọc **bảng Props** là quan trọng nhất (giống đọc datasheet).

> 📌 **Góc nhìn Embedded**: Đọc docs component React Native giống **đọc datasheet một con IC**. Bảng Props = bảng thanh ghi (register map): mỗi prop là một "cấu hình" bạn set vào component. Quen đọc datasheet rồi thì đọc docs RN cực nhanh.

---

## #3. Setup Môi Trường Khóa Học

### 1. Hai cách test ứng dụng

| Cách test | Ưu điểm | Nhược điểm |
|-----------|---------|------------|
| **Điện thoại thật** (app Expo Go) | Không tốn tài nguyên máy tính, nhanh, tiện | Chỉ test trên 1 thiết bị của bạn |
| **Điện thoại ảo** (simulator/emulator) | Test đa dạng thiết bị (to, nhỏ, nhiều đời máy) | **Tốn RAM/CPU** máy tính |

```
// Test điện thoại Android ảo → cài Android Studio
// Test điện thoại iOS ảo    → bắt buộc MacOS + cài Xcode
```

### 2. Các bước setup (thực hành theo video)

```
┌─────────────────────────────────────────────────────┐
│ 1. Cài Node.js đúng version 20.14.0                  │
│ 2. Clone source code từ Gitlab, checkout branch:     │
│      → starter  (code theo video)                    │
│      → master   (code final tham khảo)               │
│ 3. npm install  (cài thư viện)                        │
│ 4. npx expo start  → quét QR bằng Expo Go             │
└─────────────────────────────────────────────────────┘
```

> ⚠️ Cài **đúng** Node `v20.14.0`. Version Node lệch là nguyên nhân lỗi #1 của người mới.

> 💡 Máy < 8GB RAM hoặc giật lag khi mở Android Studio → ưu tiên **Expo Go** (điện thoại thật).

> 📌 **Góc nhìn Embedded**: "Điện thoại thật vs simulator" giống **nạp firmware lên board thật vs chạy trên Proteus/QEMU**. Board thật chạy đúng thực tế nhưng chỉ có board bạn đang cầm; mô phỏng thì test được nhiều "thiết bị" nhưng nặng và đôi khi sai khác hành vi thật.

---

# CHAPTER 2: CORE COMPONENTS & STYLING

> React Native KHÔNG dùng `<div>`, `<p>`, `<span>`. Thay vào đó là **Core Components** render ra UI native.

## #4. View, Text & Styles

### 1. Bảng ánh xạ HTML → React Native

| HTML (Web) | React Native | Ghi chú |
|------------|--------------|---------|
| `<div>` | `<View>` | Khối chứa (container), không hiển thị text trực tiếp |
| `<p>`, `<span>`, `<h1>` | `<Text>` | **Mọi chữ phải nằm trong `<Text>`** |
| `<input>` | `<TextInput>` | Ô nhập liệu |
| `<img>` | `<Image>` | Hiển thị ảnh |
| `<button>` | `<Button>` / `<Pressable>` | Nút bấm |
| `<ul><li>` | `<FlatList>` / `<ScrollView>` | Danh sách |

### 2. View & Text cơ bản

```jsx
import { View, Text, StyleSheet } from 'react-native';

export default function App() {
    return (
        <View style={styles.container}>
            <Text style={styles.title}>Hello React Native!</Text>
        </View>
    );
}
```

> ⚠️ **Bẫy kinh điển**: Viết chữ trực tiếp trong `<View>` → CRASH app. Mọi text **bắt buộc** bọc trong `<Text>`.
> ```jsx
> <View>Hello</View>          {/* ❌ ERROR */}
> <View><Text>Hello</Text></View>  {/* ✅ OK */}
> ```

### 3. StyleSheet (CSS trong React Native)

> Style trong RN viết bằng **object JavaScript** (camelCase), KHÔNG phải file `.css`.

```jsx
const styles = StyleSheet.create({
    container: {
        flex: 1,
        backgroundColor: '#fff',
        justifyContent: 'center',
        alignItems: 'center',
    },
    title: {
        fontSize: 24,
        fontWeight: 'bold',
        color: '#333',
    },
});
```

| CSS Web | RN StyleSheet | Khác biệt |
|---------|---------------|-----------|
| `background-color` | `backgroundColor` | **camelCase** thay vì `kebab-case` |
| `font-size: 24px` | `fontSize: 24` | **không có đơn vị** `px` (mặc định là dp) |
| `class="box"` | `style={styles.box}` | dùng object, không dùng class |
| nhiều class | `style={[styles.a, styles.b]}` | gộp style = **mảng** |

> 💡 `StyleSheet.create()` giúp tối ưu hiệu năng & gợi ý code (autocomplete). Có thể style inline `style={{ color: 'red' }}` nhưng nên tách ra `StyleSheet`.

> 📌 **Góc nhìn Embedded**: Style object = **struct cấu hình** cho một component (giống `GPIO_InitTypeDef`). Bạn điền các field (`fontSize`, `color`, `flex`) rồi "nạp" vào component qua prop `style`, y như điền struct rồi gọi `HAL_GPIO_Init(&cfg)`.

---

## #5. Sử Dụng State & Button

### 1. State với useState Hook

> **State** = bộ nhớ của component. State đổi → component **tự render lại** (re-render) → UI cập nhật.

```jsx
import { useState } from 'react';
import { View, Text, Button } from 'react-native';

export default function App() {
    const [count, setCount] = useState(0);

    return (
        <View>
            <Text>Số đếm: {count}</Text>
            <Button title="Tăng" onPress={() => setCount(count + 1)} />
        </View>
    );
}
```

### 2. Component Button

> `<Button>` của RN rất đơn giản (ít tùy biến style). Props chính:

| Prop | Ý nghĩa |
|------|---------|
| `title` | Chữ trên nút (**bắt buộc**) |
| `onPress` | Hàm chạy khi bấm |
| `color` | Màu nút |
| `disabled` | Vô hiệu hóa nút |

> ⚠️ `<Button>` **không nhận `style`** để custom giao diện. Muốn nút đẹp/tùy biến → dùng `<Pressable>` hoặc `<TouchableOpacity>` (xem #10).

> 📌 **Góc nhìn Embedded**: `onPress` là **callback của một sự kiện** — giống bạn gắn hàm vào **ngắt ngoài (EXTI interrupt)** của nút nhấn vật lý. Khác biệt cốt lõi: thay đổi `state` → UI tự vẽ lại (data-driven), bạn **không** phải tự `lcd_clear()` rồi `lcd_print()` lại như trên vi điều khiển. Đây là **reactive programming**.

---

## #6. Text Inputs

> `<TextInput>` = ô nhập liệu (giống `<input>` web). Là **controlled component**: giá trị do state quản lý.

```jsx
import { useState } from 'react';
import { View, TextInput, Text } from 'react-native';

export default function App() {
    const [name, setName] = useState("");

    return (
        <View>
            <TextInput
                style={{ borderWidth: 1, padding: 8 }}
                placeholder="Nhập tên của bạn"
                value={name}
                onChangeText={(text) => setName(text)}
            />
            <Text>Xin chào: {name}</Text>
        </View>
    );
}
```

| Prop | Ý nghĩa |
|------|---------|
| `value` | Giá trị hiện tại (lấy từ state) |
| `onChangeText` | Hàm chạy mỗi khi gõ (nhận `text`) |
| `placeholder` | Chữ gợi ý mờ |
| `keyboardType` | `numeric`, `email-address`, `phone-pad`... |
| `secureTextEntry` | `true` → ẩn ký tự (nhập password) |
| `multiline` | `true` → cho nhập nhiều dòng |

> 💡 **Luồng controlled**: gõ phím → `onChangeText` → `setName` → state đổi → re-render → `value` cập nhật. State là **"nguồn sự thật" duy nhất** (single source of truth).

> ⚠️ Khác với web: dùng `onChangeText` (nhận thẳng chuỗi text), KHÔNG phải `onChange` (nhận event).

---

## #7. Sử Dụng Array (Render List + ScrollView)

### 1. Render danh sách bằng map()

```jsx
const todos = [
    { id: 1, name: "Học React Native" },
    { id: 2, name: "Code Todo App" },
    { id: 3, name: "Ôn Embedded" },
];

return (
    <View>
        {todos.map((item) => (
            <Text key={item.id}>{item.name}</Text>
        ))}
    </View>
);
```

> ⚠️ Mỗi phần tử trong `map()` **bắt buộc** có prop `key` (duy nhất). React dùng `key` để định danh phần tử khi thêm/xóa/sửa.

### 2. ScrollView — cuộn nội dung

> `<View>` **không cuộn được**. Nếu nội dung dài hơn màn hình → dùng `<ScrollView>`.

```jsx
import { ScrollView, Text } from 'react-native';

<ScrollView>
    {todos.map((item) => (
        <Text key={item.id}>{item.name}</Text>
    ))}
</ScrollView>
```

> ⚠️ **Cảnh báo hiệu năng**: `ScrollView` render **TẤT CẢ** phần tử cùng lúc → danh sách dài (hàng trăm/nghìn item) sẽ **lag & tốn RAM**. Danh sách dài → dùng `FlatList` (#8).

> 📌 Tham khảo unique key: https://stackoverflow.com/a/29246176

> 📌 **Góc nhìn Embedded**: `ScrollView` load hết = nạp toàn bộ data vào RAM một lúc → tràn bộ nhớ trên thiết bị yếu. `FlatList` chỉ render item đang nhìn thấy = đọc dữ liệu theo kiểu **streaming/buffer**, đúng tư duy tiết kiệm RAM của dân nhúng.

---

## #8. Flat List

> `<FlatList>` = danh sách **tối ưu hiệu năng**. Chỉ render những item **đang hiển thị** trên màn hình (lazy rendering / virtualization).

```jsx
import { FlatList, Text } from 'react-native';

<FlatList
    data={todos}
    keyExtractor={(item) => item.id.toString()}
    renderItem={({ item }) => (
        <Text>{item.name}</Text>
    )}
/>
```

| Prop | Ý nghĩa |
|------|---------|
| `data` | Mảng dữ liệu |
| `renderItem` | Hàm vẽ 1 item (nhận `{ item }`) |
| `keyExtractor` | Trả về key duy nhất cho mỗi item |
| `ItemSeparatorComponent` | Component ngăn cách giữa các item |
| `ListHeaderComponent` / `ListFooterComponent` | Header / Footer danh sách |
| `onEndReached` | Hàm chạy khi cuộn gần cuối (load more / infinite scroll) |
| `horizontal` | `true` → cuộn ngang |

### So sánh ScrollView vs FlatList

| Tiêu chí | `ScrollView` | `FlatList` |
|----------|--------------|------------|
| Cách render | Render **tất cả** một lúc | Render **theo lazy** (item đang thấy) |
| Hiệu năng list dài | ❌ Lag, tốn RAM | ✅ Mượt, tiết kiệm RAM |
| Dùng khi | List ngắn, nội dung cố định | List dài, data từ API |

> 💡 **Quy tắc**: List < ~20 item cố định → `ScrollView`. List dài/động → **luôn dùng `FlatList`**.

---

# CHAPTER 3: DỰ ÁN TODO LIST

> Áp dụng kiến thức Chapter 2 để build app Todo hoàn chỉnh — bài tập thực hành kinh điển.

## #9. Todo List (Part 1)

### Logic: Thêm Todo

```jsx
import { useState } from 'react';
import { View, TextInput, Button, FlatList, Text } from 'react-native';

export default function TodoApp() {
    const [todo, setTodo] = useState("");        // input hiện tại
    const [listTodo, setListTodo] = useState([]); // danh sách todo

    const handleAddTodo = () => {
        if (!todo) return;                        // chặn thêm rỗng
        setListTodo([
            ...listTodo,                          // giữ list cũ (immutable)
            { id: Math.random(), name: todo }     // thêm todo mới
        ]);
        setTodo("");                              // reset input
    };

    return (
        <View>
            <TextInput
                value={todo}
                onChangeText={setTodo}
                placeholder="Nhập công việc..."
            />
            <Button title="Thêm" onPress={handleAddTodo} />

            <FlatList
                data={listTodo}
                keyExtractor={(item) => item.id.toString()}
                renderItem={({ item }) => <Text>{item.name}</Text>}
            />
        </View>
    );
}
```

> ⚠️ **Nguyên tắc Immutability (CỰC QUAN TRỌNG)**: KHÔNG sửa trực tiếp state. Luôn tạo **mảng/object mới**:
> ```jsx
> listTodo.push(newItem);        // ❌ SAI - mutate trực tiếp, React không re-render
> setListTodo([...listTodo, newItem]); // ✅ ĐÚNG - tạo mảng mới
> ```

> 📌 **Góc nhìn Embedded**: Quen với C, bạn hay sửa thẳng `array[i] = x`. Trong React phải **tạo bản sao mới** vì React so sánh **địa chỉ tham chiếu** (reference) để biết có cần vẽ lại không. Sửa tại chỗ → cùng địa chỉ → React tưởng "không đổi" → không re-render. Hãy coi state như **biến `const` chỉ-đọc**, mỗi lần đổi là cấp phát vùng mới.

---

## #10. Todo List (Part 2) — Pressable

### 1. Xóa Todo bằng filter()

```jsx
const handleDeleteTodo = (id) => {
    const newList = listTodo.filter((item) => item.id !== id);
    setListTodo(newList);   // tạo mảng mới không chứa item bị xóa
};
```

### 2. Pressable — bắt sự kiện bấm

> `<Pressable>` = component "bọc" bất cứ gì để biến nó thành **nút bấm được** (tùy biến giao diện thoải mái, khác `<Button>`).

```jsx
import { Pressable, Text } from 'react-native';

renderItem={({ item }) => (
    <Pressable onPress={() => handleDeleteTodo(item.id)}>
        <Text>{item.name}  ❌</Text>
    </Pressable>
)}
```

### So sánh các component "bấm được"

| Component | Đặc điểm |
|-----------|----------|
| `Button` | Đơn giản nhất, **không** custom style |
| `Pressable` | Linh hoạt nhất (khuyên dùng), biết được trạng thái `pressed` |
| `TouchableOpacity` | Bấm vào mờ đi (hiệu ứng opacity) |
| `TouchableWithoutFeedback` | Bấm không có hiệu ứng (dùng để ẩn keyboard) |

> 📌 Tham khảo: https://stackoverflow.com/a/76192331

---

## #11. Feedback với Alert & Keyboard

### 1. Alert — hộp thoại thông báo

```jsx
import { Alert } from 'react-native';

Alert.alert(
    "Cảnh báo",                          // tiêu đề
    "Bạn chưa nhập công việc!",          // nội dung
    [
        { text: "Hủy", style: "cancel" },
        { text: "OK", onPress: () => console.log("OK pressed") },
    ]
);
```

> 💡 `Alert` là **API** (không phải component) — gọi như một hàm, không render JSX.

### 2. Ẩn bàn phím khi bấm ra ngoài

> Trải nghiệm tốt: bấm ra ngoài ô input → bàn phím tự ẩn. Dùng `TouchableWithoutFeedback` + `Keyboard`.

```jsx
import { Keyboard, TouchableWithoutFeedback, View } from 'react-native';

<TouchableWithoutFeedback onPress={() => Keyboard.dismiss()}>
    <View style={{ flex: 1 }}>
        {/* toàn bộ UI */}
    </View>
</TouchableWithoutFeedback>
```

> 💡 `Keyboard.dismiss()` đóng bàn phím. `TouchableWithoutFeedback` bắt sự kiện chạm vào vùng trống.

> 📌 **Góc nhìn Embedded**: `Alert` giống bật **một dialog blocking** chờ người dùng phản hồi (giống `while(!button_pressed);` chờ xác nhận). `Keyboard.dismiss()` = chủ động "ngắt" phần cứng nhập liệu khi không cần — tư duy quản lý ngoại vi quen thuộc.

---

## #12. Flex Box (Basic)

> **Flexbox** = hệ thống bố cục (layout) chính của React Native. **Khác web**: trong RN, `flexDirection` mặc định là `column` (web là `row`).

### 1. Ba thuộc tính cốt lõi

```jsx
{
    flexDirection: 'column',     // 'column' (mặc định) | 'row'
    justifyContent: 'center',    // căn theo TRỤC CHÍNH (main axis)
    alignItems: 'center',        // căn theo TRỤC PHỤ (cross axis)
}
```

```
flexDirection: 'column' (MẶC ĐỊNH RN)        flexDirection: 'row'
┌──────────────┐                            ┌──────────────┐
│   ▢ item 1   │  ← main axis (dọc)         │ ▢   ▢   ▢    │ ← main axis (ngang)
│   ▢ item 2   │                            │ 1   2   3    │
│   ▢ item 3   │                            │              │
└──────────────┘                            └──────────────┘
   ↑ justifyContent điều khiển dọc            ↑ justifyContent điều khiển ngang
```

### 2. Giá trị justifyContent / alignItems

| Giá trị | Ý nghĩa |
|---------|---------|
| `flex-start` | Dồn về đầu |
| `center` | Căn giữa |
| `flex-end` | Dồn về cuối |
| `space-between` | Cách đều, không lề 2 đầu |
| `space-around` | Cách đều, có lề 2 đầu |
| `space-evenly` | Cách đều hoàn toàn |

### 3. flex: 1 — chiếm hết không gian

```jsx
container: { flex: 1 }   // chiếm toàn bộ màn hình còn lại
```

> 📌 Tham khảo flexbox: https://www.w3schools.com/css/css3_flexbox.asp

> 💡 **Quy tắc nhớ**:
> - `flexDirection: column` → `justifyContent` = **dọc**, `alignItems` = **ngang**
> - `flexDirection: row` → `justifyContent` = **ngang**, `alignItems` = **dọc**

> 📌 **Góc nhìn Embedded**: Nếu từng vẽ UI trên màn LCD/OLED bằng tọa độ tuyệt đối (`drawText(x, y, ...)`) thì Flexbox là một cú "giải phóng" — bạn mô tả **quan hệ** (căn giữa, dàn đều) thay vì tính từng pixel. Layout tự co giãn theo mọi kích thước màn hình, không phải hardcode `x, y` cho từng độ phân giải.

---

## #13. Sử Dụng Icons (Hoàn thiện Todo)

> Expo tích hợp sẵn nhiều bộ icon (Ionicons, MaterialIcons, FontAwesome, AntDesign...).

```jsx
import { AntDesign, Ionicons } from '@expo/vector-icons';

<AntDesign name="delete" size={24} color="red" />
<Ionicons name="add-circle" size={30} color="green" />
```

| Prop | Ý nghĩa |
|------|---------|
| `name` | Tên icon (tra tại trang dưới) |
| `size` | Kích thước |
| `color` | Màu |

> 📌 **Tra tên icon**: https://docs.expo.dev/guides/icons/ và https://icons.expo.fyi/Index

> 💡 Thay nút "❌ Xóa" text bằng `<AntDesign name="delete" />` để Todo App đẹp & chuyên nghiệp hơn → hoàn thiện dự án Todo.

---

# CHAPTER 4: FONTS & NAVIGATION

> Tùy biến font chữ và **điều hướng nhiều màn hình** (multi-screen app).

## #14. Sử Dụng Fonts

> Dùng `expo-font` để load font tùy chỉnh + `expo-splash-screen` để giữ màn hình chờ cho tới khi font load xong.

### 1. Cài thư viện (đúng version!)

```bash
npm i --save-exact expo-font@12.0.9 expo-splash-screen@0.27.5
```

### 2. Load font ở Root (`_layout.jsx` / `App.js`)

```jsx
import { useFonts } from 'expo-font';
import * as SplashScreen from 'expo-splash-screen';
import { useEffect } from 'react';

// Giữ splash screen, không ẩn vội
SplashScreen.preventAutoHideAsync();

export default function RootLayout() {
    const [loaded, error] = useFonts({
        'Inter-Black': require('./assets/fonts/Inter-Black.otf'),
    });

    useEffect(() => {
        if (loaded || error) {
            SplashScreen.hideAsync();   // font xong → ẩn splash
        }
    }, [loaded, error]);

    if (!loaded && !error) {
        return null;                    // chưa xong → chưa render UI
    }

    return (
        /* ... UI của bạn ... */
    );
}
```

### 3. Dùng font

```jsx
<Text style={{ fontFamily: 'Inter-Black' }}>Chữ với font tùy chỉnh</Text>
```

> 📌 Tài liệu: https://docs.expo.dev/develop/user-interface/fonts/
> 📌 Font dùng trong video: [Google Drive](https://drive.google.com/drive/folders/1pGvK69Y37GHmmhYL2fpD4mfMwvBfdsoY?usp=sharing)

> 📌 **Góc nhìn Embedded**: `SplashScreen.preventAutoHideAsync()` rồi load font xong mới `hideAsync()` = **chặn khởi động** cho tới khi tài nguyên sẵn sàng — y hệt `while(!sensor_ready);` trong `setup()` trước khi vào `loop()`. Đảm bảo không vẽ UI thiếu font (giống không đọc cảm biến khi chưa init xong).

---

## #15. Giới Thiệu Navigation

> App thật có **nhiều màn hình** (Home, Detail, Settings...). **React Navigation** là thư viện điều hướng phổ biến nhất.

### 1. Cài thư viện (Stack Navigator)

```bash
npm i --save-exact @react-navigation/native@6.1.18 @react-navigation/native-stack@6.10.1
npm i --save-exact react-native-screens@3.31.1 react-native-safe-area-context@4.10.5
```

### 2. Các loại Navigator

| Navigator | Kiểu điều hướng | Dùng khi |
|-----------|-----------------|----------|
| **Stack** | Chồng màn hình (push/pop, có nút back) | Luồng Home → Detail → ... |
| **Drawer** | Menu kéo từ cạnh trái | Menu chính của app |
| **Tab** | Thanh tab dưới đáy | Chuyển nhanh giữa các mục lớn |

### 3. Global styles (biến dùng chung)

> Tạo file chứa màu sắc / spacing dùng chung toàn app (giống biến `#define` trong C).

```jsx
// constants/globalStyles.js
export const APP_COLOR = {
    ORANGE: "#f4511e",
    GREY: "#ccc",
};
```

> 📌 Tài liệu: https://reactnative.dev/docs/navigation

---

## #16. Hello React Navigation

> Bọc app trong `NavigationContainer` và khai báo Stack.

```jsx
import { NavigationContainer } from '@react-navigation/native';
import { createNativeStackNavigator } from '@react-navigation/native-stack';

import HomeScreen from './screens/HomeScreen';
import DetailScreen from './screens/DetailScreen';

const Stack = createNativeStackNavigator();

export default function App() {
    return (
        <NavigationContainer>
            <Stack.Navigator initialRouteName="Home">
                <Stack.Screen name="Home" component={HomeScreen} />
                <Stack.Screen name="Detail" component={DetailScreen} />
            </Stack.Navigator>
        </NavigationContainer>
    );
}
```

| Thành phần | Vai trò |
|------------|---------|
| `NavigationContainer` | Bọc ngoài cùng (bắt buộc, chỉ 1 lần) |
| `Stack.Navigator` | Khai báo nhóm màn hình + cấu hình |
| `Stack.Screen` | 1 màn hình (`name` = tên route, `component` = màn hình) |
| `initialRouteName` | Màn hình mở đầu tiên |

> 📌 Tài liệu: https://reactnavigation.org/docs/hello-react-navigation

> 📌 **Góc nhìn Embedded**: `Stack.Navigator` chính là một **stack thật** (LIFO). `navigate()` = `push` lên stack, nút Back = `pop`. Giống call stack khi gọi hàm lồng nhau trên vi điều khiển: vào hàm con thì push, return thì pop.

---

## #17. Moving Between Screens

> Mọi màn hình khai báo trong `Stack.Screen` **tự động nhận** prop `navigation`.

```jsx
// Trong HomeScreen
function HomeScreen({ navigation }) {
    return (
        <Button
            title="Sang Detail"
            onPress={() => navigation.navigate('Detail')}
        />
    );
}
```

### Hook useNavigation (component con sâu)

> Component lồng sâu không có sẵn prop `navigation` → dùng hook `useNavigation`.

```jsx
import { useNavigation } from '@react-navigation/native';

function MyButton() {
    const navigation = useNavigation();
    return <Button title="Go" onPress={() => navigation.navigate('Detail')} />;
}
```

| Method | Tác dụng |
|--------|----------|
| `navigation.navigate('X')` | Sang màn hình X |
| `navigation.push('X')` | Chồng thêm 1 màn X mới (kể cả đang ở X) |
| `navigation.goBack()` | Quay lại màn trước |
| `navigation.popToTop()` | Về màn đầu tiên của stack |

> 📌 Tài liệu: https://reactnavigation.org/docs/navigating · https://reactnavigation.org/docs/use-navigation · https://stackoverflow.com/a/76779527

---

## #18. Passing Parameters To Routes

> Truyền dữ liệu **từ màn này sang màn khác** qua tham số thứ 2 của `navigate`.

```jsx
// Màn gửi (Home)
navigation.navigate('Detail', { itemId: 42, name: "ESP32" });

// Màn nhận (Detail) — cách 1: qua prop route
function DetailScreen({ route }) {
    const { itemId, name } = route.params;
    return <Text>ID: {itemId} - Tên: {name}</Text>;
}

// Cách 2: dùng hook useRoute
import { useRoute } from '@react-navigation/native';
const route = useRoute();
const { itemId } = route.params;
```

> 💡 `route.params` = object chứa data được truyền. Nếu có thể không tồn tại → dùng optional chaining `route.params?.itemId`.

> 📌 Tài liệu: https://reactnavigation.org/docs/params · https://reactnavigation.org/docs/use-route

> 📌 **Góc nhìn Embedded**: `navigate('Detail', {...})` = **gọi hàm và truyền tham số**; `route.params` ở màn đích = các đối số nhận được. Giống truyền struct/pointer qua hàng đợi (queue) giữa các task trong RTOS để chuyển dữ liệu giữa các "ngữ cảnh".

---

## #19. Drawer Navigator

> Menu **kéo ra từ cạnh** màn hình (hamburger menu ☰).

### Cài thư viện

```bash
npm i --save-exact @react-navigation/drawer@6.7.2
npm i --save-exact react-native-gesture-handler@2.16.1 react-native-reanimated@3.10.1
```

```jsx
import { createDrawerNavigator } from '@react-navigation/drawer';

const Drawer = createDrawerNavigator();

<NavigationContainer>
    <Drawer.Navigator>
        <Drawer.Screen name="Home" component={HomeScreen} />
        <Drawer.Screen name="Settings" component={SettingsScreen} />
    </Drawer.Navigator>
</NavigationContainer>
```

> ⚠️ `react-native-reanimated` cần thêm cấu hình `babel.config.js` (plugin `react-native-reanimated/plugin` để **cuối cùng** trong mảng plugins). Làm đúng như video để tránh lỗi.

> 📌 Tài liệu: https://reactnavigation.org/docs/drawer-navigator

---

## #20. Custom Header

> Tùy biến thanh header (màu, tiêu đề, nút trái/phải).

```jsx
<Stack.Screen
    name="Home"
    component={HomeScreen}
    options={{
        title: 'Trang chủ',
        headerStyle: { backgroundColor: '#f4511e' },
        headerTintColor: '#fff',                       // màu chữ + nút back
        headerTitleStyle: { fontWeight: 'bold' },
        headerRight: () => (
            <Ionicons name="settings" size={24} color="#fff" />
        ),
    }}
/>
```

| Option | Tác dụng |
|--------|----------|
| `title` | Tiêu đề header |
| `headerStyle` | Style nền header |
| `headerTintColor` | Màu chữ & nút back |
| `headerRight` / `headerLeft` | Component bên phải/trái |
| `headerShown: false` | Ẩn hẳn header |

> 📌 Tra icon: https://icons.expo.fyi/Index

---

# CHAPTER 5: IMAGES, MODAL & HOÀN THIỆN

## #21. Sử Dụng Images

### 1. Image (ảnh local & ảnh từ URL)

```jsx
import { Image } from 'react-native';

// Ảnh local (dùng require)
<Image source={require('./assets/logo.png')} style={{ width: 100, height: 100 }} />

// Ảnh từ URL (bắt buộc khai báo width/height)
<Image
    source={{ uri: 'https://example.com/img.png' }}
    style={{ width: 100, height: 100 }}
/>
```

> ⚠️ Ảnh từ `uri` (URL) **bắt buộc** có `width` & `height` trong style, nếu không sẽ **không hiển thị**.

### 2. ImageBackground (ảnh nền)

```jsx
import { ImageBackground } from 'react-native';

<ImageBackground source={require('./assets/bg.png')} style={{ flex: 1 }}>
    <Text>Nội dung trên nền ảnh</Text>
</ImageBackground>
```

### 3. SafeAreaView & StatusBar (fix header bị che)

> Trên iPhone tai thỏ / Android có notch → nội dung bị che. Dùng `react-native-safe-area-context`.

```jsx
import { SafeAreaView } from 'react-native-safe-area-context';

<SafeAreaView style={{ flex: 1 }}>
    {/* nội dung không bị tai thỏ che */}
</SafeAreaView>
```

> 📌 Tài liệu: [Image](https://reactnative.dev/docs/image) · [ImageBackground](https://reactnative.dev/docs/imagebackground) · [StatusBar](https://docs.expo.dev/guides/configuring-statusbar/) · [SafeAreaContext](https://docs.expo.dev/versions/latest/sdk/safe-area-context/)
> 📌 Ảnh dùng trong video: [Google Drive](https://drive.google.com/drive/folders/1pGvK69Y37GHmmhYL2fpD4mfMwvBfdsoY?usp=sharing)

---

## #22. Sử Dụng Modal & Form

> `<Modal>` = cửa sổ pop-up nổi trên màn hình (dùng cho form thêm/sửa, xác nhận...).

### 1. Modal cơ bản

```jsx
import { Modal, View, Text, Pressable, Alert } from 'react-native';
import { useState } from 'react';

const [modalVisible, setModalVisible] = useState(false);

<Modal
    animationType="slide"          // 'slide' | 'fade' | 'none'
    transparent={true}             // nền trong suốt
    visible={modalVisible}         // điều khiển ẩn/hiện bằng state
    onRequestClose={() => {        // bấm nút back vật lý (Android)
        Alert.alert('Modal has been closed.');
        setModalVisible(!modalVisible);
    }}>
    <View style={styles.centeredView}>
        <View style={styles.modalView}>
            <Text style={styles.modalText}>Hello World!</Text>
            <Pressable
                style={[styles.button, styles.buttonClose]}
                onPress={() => setModalVisible(!modalVisible)}>
                <Text style={styles.textStyle}>Hide Modal</Text>
            </Pressable>
        </View>
    </View>
</Modal>
```

### 2. Style cho Modal (overlay căn giữa + đổ bóng)

```jsx
const styles = StyleSheet.create({
    centeredView: {
        flex: 1,
        justifyContent: 'center',
        alignItems: 'center',
        marginTop: 22,
    },
    modalView: {
        margin: 20,
        backgroundColor: 'white',
        borderRadius: 20,
        padding: 35,
        alignItems: 'center',
        shadowColor: '#000',
        shadowOffset: { width: 0, height: 2 },
        shadowOpacity: 0.25,
        shadowRadius: 4,
        elevation: 5,            // đổ bóng trên Android
    },
    button: {
        borderRadius: 20,
        padding: 10,
        elevation: 2,
    },
    buttonOpen: { backgroundColor: '#F194FF' },
    buttonClose: { backgroundColor: '#2196F3' },
    textStyle: {
        color: 'white',
        fontWeight: 'bold',
        textAlign: 'center',
    },
    modalText: {
        marginBottom: 15,
        textAlign: 'center',
    },
});
```

| Prop Modal | Ý nghĩa |
|-----------|---------|
| `visible` | `true`/`false` — ẩn/hiện (điều khiển bằng state) |
| `animationType` | `slide` / `fade` / `none` |
| `transparent` | `true` → thấy nền phía sau |
| `onRequestClose` | Chạy khi bấm nút back vật lý (Android) — **bắt buộc** |

> 💡 **Bóng đổ (shadow)**: iOS dùng `shadowColor/shadowOffset/shadowOpacity/shadowRadius`, Android dùng `elevation`. Muốn đổ bóng cả 2 nền → khai báo **cả hai**.

> 📌 Tài liệu: https://reactnative.dev/docs/modal

---

## #23. Hoàn Thiện Dự Án

> Ghép tất cả: Form (Modal) thêm việc → FlatList hiển thị → Pressable + Icon xóa → Style đẹp.

```jsx
// Hàm tiện ích sinh số ngẫu nhiên (vd: tạo id, màu random...)
function randomInteger(min, max) {
    return Math.floor(Math.random() * (max - min + 1)) + min;
}
```

> 💡 Checklist hoàn thiện một app cơ bản:
> - ✅ Thêm / xóa item (state + immutable update)
> - ✅ FlatList hiển thị danh sách
> - ✅ Modal + Form nhập liệu
> - ✅ Alert validate (chặn nhập rỗng)
> - ✅ Icon + style chỉn chu
> - ✅ SafeAreaView (không bị tai thỏ che)
> - ✅ Ẩn keyboard khi bấm ra ngoài

---

## #24. Tổng Kết

> Sau khóa Basic, bạn đã nắm: Core Components, Styling (Flexbox), State/Props, List, Navigation, Modal — **đủ để build app CRUD cơ bản**.

📚 Học thêm:
- 🌐 React Native: https://reactnative.dev/
- 🌐 Expo: https://docs.expo.dev/

> 🧠 **Triết lý**: "Learn once, write anywhere" — bạn đã có **tư duy React** rồi, giờ áp dụng được cho cả web (React.js) lẫn mobile (React Native).

---

# 🎁 BONUS

## #B1. React Native cho dân Embedded (Bảng so sánh)

> Bảng "dịch" khái niệm React Native sang ngôn ngữ nhúng quen thuộc — đọc xong vào nghề nhanh hơn.

| Khái niệm React Native | Tương đương Embedded (C/Arduino/RTOS) | Giải thích ngắn |
|------------------------|----------------------------------------|------------------|
| `state` (useState) | Biến global / thanh ghi trạng thái | Lưu trạng thái; đổi → hệ thống phản ứng |
| Đổi state → re-render | Cập nhật biến → vẽ lại LCD trong `loop()` | RN tự lo việc vẽ lại (data-driven) |
| `props` | Tham số truyền vào hàm | Cha truyền data xuống con (read-only) |
| Component | Module / hàm tái sử dụng | Khối UI đóng gói, dùng lại nhiều nơi |
| `useEffect(() => {}, [])` | `setup()` (chạy 1 lần) | Init khi component mount |
| `useEffect` có cleanup | `setup()` + hàm hủy khi tắt | Dọn tài nguyên khi unmount |
| `onPress` callback | ISR (hàm phục vụ ngắt) của nút nhấn | Gắn hàm vào sự kiện |
| `Stack.Navigator` | Call stack (LIFO) | push màn hình / pop khi back |
| `navigate(name, params)` | Gửi message + data qua queue (RTOS) | Chuyển ngữ cảnh + truyền dữ liệu |
| Immutability (`[...arr]`) | Cấp phát vùng nhớ mới thay vì sửa tại chỗ | RN so sánh reference để biết có đổi |
| `FlatList` (lazy render) | Đọc dữ liệu theo buffer/streaming | Tiết kiệm RAM, không load hết một lúc |
| Expo | Arduino core / HAL layer | Bọc phần phức tạp, viết code cấp cao |
| `StyleSheet` object | Struct cấu hình (`GPIO_InitTypeDef`) | Điền field rồi "nạp" vào component |
| `SplashScreen` chờ font | `while(!ready);` trong init | Chặn đến khi tài nguyên sẵn sàng |

> 💡 **Khác biệt tư duy lớn nhất**: Embedded là **imperative** (bạn ra lệnh từng bước: clear → vẽ lại). React Native là **declarative** (bạn mô tả "UI nên trông như thế nào với state này", RN tự lo việc vẽ). Quen rồi sẽ thấy đỡ việc hơn nhiều.

---

## #B2. Core Components Cheat Sheet

```jsx
import {
    View,        // <div> — khối chứa
    Text,        // <p>/<span> — mọi chữ phải trong đây
    TextInput,   // <input> — ô nhập (onChangeText)
    Image,       // <img> — ảnh (require local / {uri})
    ImageBackground, // ảnh nền
    ScrollView,  // cuộn (list ngắn)
    FlatList,    // list dài (tối ưu)
    Button,      // nút đơn giản (không style)
    Pressable,   // nút tùy biến (khuyên dùng)
    TouchableOpacity, // nút có hiệu ứng mờ
    Modal,       // pop-up
    Alert,       // API hộp thoại (không phải component)
    Keyboard,    // API điều khiển bàn phím
    StyleSheet,  // tạo style object
} from 'react-native';

import { SafeAreaView } from 'react-native-safe-area-context'; // tránh tai thỏ
import { AntDesign, Ionicons } from '@expo/vector-icons';      // icons
```

---

## #B3. Styling & Flexbox Cheat Sheet

```jsx
// FLEXBOX (mặc định flexDirection: 'column' trong RN!)
{ flex: 1 }                          // chiếm hết không gian còn lại
{ flexDirection: 'row' }             // xếp ngang (web mặc định)
{ justifyContent: 'center' }         // căn theo trục chính
{ alignItems: 'center' }             // căn theo trục phụ
{ gap: 10 }                          // khoảng cách giữa các con

// KÍCH THƯỚC & KHOẢNG CÁCH (không có px!)
{ width: 100, height: 50 }
{ padding: 16, margin: 8 }
{ paddingHorizontal: 12, paddingVertical: 8 }

// VIỀN & BO GÓC
{ borderWidth: 1, borderColor: '#ccc', borderRadius: 8 }

// CHỮ
{ fontSize: 16, fontWeight: 'bold', color: '#333', textAlign: 'center' }

// BÓNG (iOS + Android)
{ shadowColor: '#000', shadowOpacity: 0.25, shadowRadius: 4,
  shadowOffset: { width: 0, height: 2 }, elevation: 5 }

// GỘP NHIỀU STYLE
style={[styles.base, isActive && styles.active]}
```

> ⚠️ **3 khác biệt CSS web → RN**: (1) camelCase, (2) không đơn vị `px`, (3) `flexDirection` mặc định `column`.

---

## #B4. Navigation Cheat Sheet

```jsx
// SETUP
import { NavigationContainer } from '@react-navigation/native';
import { createNativeStackNavigator } from '@react-navigation/native-stack';
const Stack = createNativeStackNavigator();

<NavigationContainer>
    <Stack.Navigator initialRouteName="Home">
        <Stack.Screen name="Home" component={Home} options={{ title: 'Trang chủ' }} />
        <Stack.Screen name="Detail" component={Detail} />
    </Stack.Navigator>
</NavigationContainer>

// ĐIỀU HƯỚNG
navigation.navigate('Detail', { id: 1 });   // sang màn + truyền data
navigation.goBack();                          // quay lại

// NHẬN PARAMS
const { id } = route.params;                  // qua prop route
const { id } = useRoute().params;             // qua hook

// HOOK (component con sâu)
const navigation = useNavigation();
```

| Thư viện | Version (khóa học) |
|----------|--------------------|
| `@react-navigation/native` | `6.1.18` |
| `@react-navigation/native-stack` | `6.10.1` |
| `@react-navigation/drawer` | `6.7.2` |
| `react-native-screens` | `3.31.1` |
| `react-native-safe-area-context` | `4.10.5` |
| `react-native-gesture-handler` | `2.16.1` |
| `react-native-reanimated` | `3.10.1` |
| `expo-font` | `12.0.9` |
| `expo-splash-screen` | `0.27.5` |

---

## #B5. Expo & Lệnh Thường Dùng

```bash
# TẠO DỰ ÁN MỚI
npx create-expo-app@latest MyApp
cd MyApp

# CHẠY DỰ ÁN
npx expo start              # mở Metro bundler → quét QR bằng Expo Go
npx expo start --android    # mở thẳng Android emulator
npx expo start --ios        # mở thẳng iOS simulator (cần MacOS)
npx expo start -c           # xóa cache khi bị lỗi lạ

# CÀI THƯ VIỆN (đúng version → ít lỗi)
npm i --save-exact <package>@<version>
npx expo install <package>  # Expo tự chọn version tương thích

# DỌN DẸP KHI LỖI
rm -rf node_modules && npm install
```

> 💡 **Mẹo gỡ lỗi**: 90% lỗi của người mới do (1) sai version Node, (2) sai version thư viện, (3) cache. Thử `npx expo start -c` và cài đúng version trước khi hoảng.

---

## #B6. Cấu Trúc Thư Mục & Roadmap Học Tiếp

### Cấu trúc thư mục gợi ý

```
MyApp/
├── assets/
│   ├── fonts/          # font .otf/.ttf
│   └── images/         # ảnh local
├── components/         # component tái sử dụng (Button, Card...)
├── screens/            # các màn hình (HomeScreen, DetailScreen...)
├── navigation/         # cấu hình Stack/Drawer/Tab
├── constants/          # globalStyles, colors, config
├── App.js              # điểm vào (entry point)
└── package.json
```

### Roadmap sau khóa React Native Basic

```
┌─────────────────────────────────────────────────────┐
│ SAU REACT NATIVE BASIC                               │
├─────────────────────────────────────────────────────┤
│ 1. TypeScript với React Native                       │
│    - Type-safe, gần như bắt buộc khi đi làm          │
├─────────────────────────────────────────────────────┤
│ 2. Expo Router (file-based routing)                  │
│    - Điều hướng kiểu Next.js, hiện đại               │
├─────────────────────────────────────────────────────┤
│ 3. Gọi API & State Management                        │
│    - Axios / Fetch, React Query (TanStack)           │
│    - Redux Toolkit / Zustand                         │
├─────────────────────────────────────────────────────┤
│ 4. Native Features                                   │
│    - Camera, Location, Notifications, AsyncStorage   │
│    - expo-* modules (sensor, BLE...)                 │
├─────────────────────────────────────────────────────┤
│ 5. Backend cho Mobile                                │
│    - Node.js + Express, Firebase, REST/GraphQL       │
├─────────────────────────────────────────────────────┤
│ 6. Build & Deploy                                    │
│    - EAS Build → file .apk/.ipa                      │
│    - Đăng Google Play / App Store                    │
└─────────────────────────────────────────────────────┘
```

### 🔧 Roadmap riêng cho dân Embedded (IoT App)

```
┌─────────────────────────────────────────────────────┐
│ KẾT HỢP REACT NATIVE + EMBEDDED                      │
├─────────────────────────────────────────────────────┤
│ • react-native-ble-plx  → giao tiếp BLE với ESP32    │
│ • MQTT (mqtt.js / Paho) → app điều khiển thiết bị    │
│ • WebSocket / Socket.IO → real-time với firmware     │
│ • Ý tưởng: App điều khiển ESP32 Smart Home / Lock    │
│   (rất hợp capstone Smart Lock của bạn!)             │
└─────────────────────────────────────────────────────┘
```

> 💡 **Gợi ý cho bạn (dân Embedded)**: Project React Native + ESP32 cực kỳ "ăn điểm" portfolio — ví dụ app mobile điều khiển khóa thông minh qua BLE/MQTT, hiển thị trạng thái cảm biến real-time. Đây là điểm giao thoa Mobile ↔ IoT mà rất ít người làm được cả 2 đầu.

---

## 🎓 LỜI KẾT

> 💪 **36 videos** đưa bạn từ số 0 đến app mobile chạy trên cả Android & iOS.

Tài liệu này tổng hợp từ:
- 📺 Khóa **Tự Học React Native (Basic)** của **Hỏi Dân IT với Eric** — 24 Bước / 36 videos
- 🎯 Tài liệu chính thức: https://reactnative.dev/ và https://docs.expo.dev/
- 🔧 Bổ sung **góc nhìn Embedded** xuyên suốt cho dân nhúng

### Lời khuyên cuối

1. **Code theo video** — không học chay (cài đúng Node `20.14.0` + version thư viện)
2. **Nắm vững Core Components** — `View`, `Text`, `FlatList` là nền tảng mọi app
3. **Master Flexbox** — 90% layout RN nằm ở `flexDirection`, `justifyContent`, `alignItems`
4. **Hiểu Immutability** — luôn `[...arr]` / `{...obj}`, đừng mutate state (nguồn gốc nhiều bug)
5. **Học React.js (web) song song** — cùng tư duy, củng cố lẫn nhau
6. **Push GitHub thường xuyên** — vừa thực hành Git vừa làm portfolio
7. **Build project thật** — Todo App là khởi đầu; mục tiêu: app điều khiển ESP32 của bạn

### Tài nguyên học thêm

- 🌐 [React Native Docs](https://reactnative.dev/) — tài liệu chính thức
- 🌐 [Expo Docs](https://docs.expo.dev/) — framework dùng trong khóa
- 🌐 [React Navigation](https://reactnavigation.org/) — điều hướng
- 🌐 [Expo Icons](https://icons.expo.fyi/) — tra tên icon
- 📺 [Hỏi Dân IT - YouTube](https://www.youtube.com/@hoidanit) — khóa học gốc
- 🌐 [hoidanit.vn](https://hoidanit.vn/) — website chính thức tác giả

### Ý tưởng project luyện tập React Native

1. **Todo App** — như trong khóa (State, FlatList, Modal)
2. **Weather App** — gọi API, hiển thị thời tiết
3. **Note App** — CRUD + AsyncStorage (lưu local)
4. **Movie App** — TMDB API, FlatList, infinite scroll
5. **Shopping Cart** — Redux/Zustand, navigation nhiều màn
6. **🔧 IoT Control App** — điều khiển ESP32 qua BLE/MQTT (hợp dân Embedded!)
7. **Chat App** — Socket.IO real-time

⭐ **Star** repo này nếu hữu ích nhé! Chúc bạn làm chủ React Native và build được app điều khiển thiết bị nhúng của riêng mình! 📱🔧🚀

---

> 📝 *Tài liệu được tổng hợp lại để học tập và lưu trữ. Nội dung gốc thuộc về **Hỏi Dân IT với Eric** (https://hoidanit.vn) và được bổ sung thêm kiến thức React Native chuẩn từ tài liệu chính thức https://reactnative.dev — kèm góc nhìn dành cho dân Embedded.*

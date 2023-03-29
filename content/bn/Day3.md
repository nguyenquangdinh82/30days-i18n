# st.button

`st.button` একটি বোতাম উইজেট প্রদর্শনের অনুমতি দেয়।

## আমরা কি নির্মাণ করছি?

একটি সাধারণ অ্যাপ যা শর্তসাপেক্ষে সঞ্চালিত করে বিকল্প বার্তাগুলিকে প্রিন্ট আউট করে তা নির্ভর করে বোতামটি চাপানো হয়েছে কি না।

অ্যাপের প্রবাহ:

1. ডিফল্টরূপে, অ্যাপটি `গুডবাই` প্রিন্ট করে
2. বাটন ক্লিক করার পরে, অ্যাপটি 'কেন হ্যালো সেখানে' বিকল্প বার্তা প্রদর্শন করে

## ডেমো অ্যাপ

স্থাপন করা স্ট্রিমলিট অ্যাপটি নীচের লিঙ্কে দেখানোর মতো দেখতে হবে: 

[![স্ট্রিমলিট অ্যাপ](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/dataprofessor/st.button/)

## কোড

উপরে উল্লিখিত অ্যাপটি বাস্তবায়ন করার কোড এখানে:

```python
import streamlit as st

st.header('st.button')

if st.button('Say hello'):
     st.write('Why hello there')
else:
     st.write('Goodbye')
```

## লাইন-বাই-লাইন ব্যাখ্যা

স্ট্রিমলিট অ্যাপ তৈরী করার জন্য প্রথম জিনিসটি হলো `streamlit` লাইব্রেরি `st` হিসেবে ইম্পোর্ট করা:

```python
import streamlit as st
```

এটি অ্যাপের জন্য একটি শিরোনাম পাঠ্য তৈরি করে অনুসরণ করা হয়:

```python
st.header('st.button')
```

পরবর্তী, আমরা বিকল্প বার্তা প্রিন্ট করার জন্য শর্তসাপেক্ষ বিবৃতি ব্যবহার করব `if` এবং `else`।

```python
if st.button('Say hello'):
     st.write('Why hello there')
else:
     st.write('Goodbye')
```

আমরা উপরের কোড বক্স থেকে দেখতে পাচ্ছি, `st.button()` কমান্ডটি `সে হ্যালো` এর `লেবেল` ইনপুট আর্গুমেন্ট গ্রহণ করে, যা বোতামটি প্রদর্শন করে এমন পাঠ্য।

`st.write` কমান্ডটি `কেন হ্যালো সেখানে` বা `গুডবাই` এর টেক্সট মেসেজ প্রিন্ট করতে ব্যবহার করা হয় বোতামটি ক্লিক করা হয়েছে কি না তার উপর নির্ভর করে, যা এর মাধ্যমে প্রয়োগ করা হয়:


```python
st.write('Why hello there')
```

এবং

```python
st.write('Goodbye')
```

এটি লক্ষ করা গুরুত্বপূর্ণ যে উপরের `st.write` বিবৃতিগুলিকে `if` এবং `else` শর্তের অধীনে বার্তাগুলির বিকল্প প্রদর্শনের উপরে উল্লিখিত প্রক্রিয়া সম্পাদন করার জন্য স্থাপন করা হয়েছে

## পরবর্তী পদক্ষেপ

এখন যেহেতু আপনি স্থানীয়ভাবে স্ট্রিমলিট অ্যাপ তৈরি করেছেন, এটিকে [স্ট্রিমলিট কমিউনিটি ক্লাউড](https://streamlit.io/cloud) এ স্থাপন করার সময় এসেছে যা একটি আসন্ন চ্যালেঞ্জে শীঘ্রই ব্যাখ্যা করা হবে।

কারণ এটি আপনার চ্যালেঞ্জের প্রথম সপ্তাহ, আমরা এই ওয়েবপৃষ্ঠার ভিতরেই সম্পূর্ণ কোড (উপরের কোড বক্সে দেখানো হয়েছে) এবং সমাধান (ডেমো অ্যাপ) প্রদান করি।

পরবর্তী চ্যালেঞ্জগুলিতে এগিয়ে যাওয়ার জন্য, আপনাকে প্রথমে স্ট্রিমলিট অ্যাপটি প্রয়োগ করার চেষ্টা করার পরামর্শ দেওয়া হচ্ছে।

আপনি আটকে গেলে চিন্তা করবেন না, আপনি সবসময় সমাধানটি উঁকি দিতে পারেন।

## তথ্যসূত্র

স্ট্রিমলিট API ডকুমেন্টেশনে [`st.button`](https://docs.streamlit.io/library/api-reference/widgets/st.button) সম্পর্কে পড়ুন।

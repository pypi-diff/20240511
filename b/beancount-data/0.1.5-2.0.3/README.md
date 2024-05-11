# Comparing `tmp/beancount-data-0.1.5.tar.gz` & `tmp/beancount_data-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount-data-0.1.5.tar", max compression
+gzip compressed data, was "beancount_data-2.0.3.tar", max compression
```

## Comparing `beancount-data-0.1.5.tar` & `beancount_data-2.0.3.tar`

### file list

```diff
@@ -1,5 +1,32 @@
--rw-r--r--   0        0        0     1072 2023-03-22 20:50:24.517483 beancount-data-0.1.5/LICENSE
--rw-r--r--   0        0        0     3740 2023-03-22 20:50:24.517483 beancount-data-0.1.5/beancount_data/__init__.py
--rw-r--r--   0        0        0      382 2023-03-22 20:50:24.517483 beancount-data-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      655 2023-03-22 20:50:33.056690 beancount-data-0.1.5/setup.py
--rw-r--r--   0        0        0      461 2023-03-22 20:50:33.056882 beancount-data-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-01-04 04:14:37.542930 beancount_data-2.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/__init__.py
+-rw-r--r--   0        0        0     3607 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/data_types.py
+-rw-r--r--   0        0        0        0 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/__init__.py
+-rw-r--r--   0        0        0     1763 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Amount.py
+-rw-r--r--   0        0        0     2990 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Balance.py
+-rw-r--r--   0        0        0     2684 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Beancount.py
+-rw-r--r--   0        0        0      188 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Booking.py
+-rw-r--r--   0        0        0     1323 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Close.py
+-rw-r--r--   0        0        0     1375 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Commodity.py
+-rw-r--r--   0        0        0     2664 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Cost.py
+-rw-r--r--   0        0        0     3636 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/CostSpec.py
+-rw-r--r--   0        0        0      163 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/CostTypes.py
+-rw-r--r--   0        0        0     2547 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Custom.py
+-rw-r--r--   0        0        0     3347 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/CustomValue.py
+-rw-r--r--   0        0        0      182 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/CustomValueType.py
+-rw-r--r--   0        0        0     1035 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Date.py
+-rw-r--r--   0        0        0     3885 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Document.py
+-rw-r--r--   0        0        0     3440 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Entry.py
+-rw-r--r--   0        0        0      289 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/EntryPayload.py
+-rw-r--r--   0        0        0     1757 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Event.py
+-rw-r--r--   0        0        0     4825 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/MapItem.py
+-rw-r--r--   0        0        0      189 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/MapValueType.py
+-rw-r--r--   0        0        0     3765 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Note.py
+-rw-r--r--   0        0        0     2790 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Open.py
+-rw-r--r--   0        0        0     1769 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Pad.py
+-rw-r--r--   0        0        0     5025 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Posting.py
+-rw-r--r--   0        0        0     1749 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Price.py
+-rw-r--r--   0        0        0     5673 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Transaction.py
+-rw-r--r--   0        0        0        0 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/__init__.py
+-rw-r--r--   0        0        0      487 2024-01-04 04:14:37.542930 beancount_data-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 beancount_data-2.0.3/PKG-INFO
```

### Comparing `beancount-data-0.1.5/LICENSE` & `beancount_data-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount-data-0.1.5/beancount_data/__init__.py` & `beancount_data-2.0.3/beancount_data/data_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,38 +64,38 @@
     currency: typing.Optional[str]
     date: datetime.date
     label: typing.Optional[str]
     merge: typing.Optional[bool]
 
 
 class Open(EntryBase):
-    entry_type: EntryType = Field(EntryType.OPEN, const=EntryType.OPEN)
+    entry_type: EntryType = Field(EntryType.OPEN, const=True)
     account: Account
     currencies: typing.Optional[typing.List[str]]
     booking: typing.Optional[Booking]
 
 
 class Close(EntryBase):
-    entry_type: EntryType = Field(EntryType.CLOSE, const=EntryType.CLOSE)
+    entry_type: EntryType = Field(EntryType.CLOSE, const=True)
     account: Account
 
 
 class Commodity(EntryBase):
-    entry_type: EntryType = Field(EntryType.COMMODITY, const=EntryType.COMMODITY)
+    entry_type: EntryType = Field(EntryType.COMMODITY, const=True)
     currency: str
 
 
 class Pad(EntryBase):
-    entry_type: EntryType = Field(EntryType.PAD, const=EntryType.PAD)
+    entry_type: EntryType = Field(EntryType.PAD, const=True)
     account: Account
     source_account: str
 
 
 class Balance(EntryBase):
-    entry_type: EntryType = Field(EntryType.BALANCE, const=EntryType.BALANCE)
+    entry_type: EntryType = Field(EntryType.BALANCE, const=True)
     account: Account
     amount: Amount
     tolerance: typing.Optional[decimal.Decimal]
     diff_amount: typing.Optional[Amount]
 
 
 class Posting(BaseModel):
@@ -104,53 +104,53 @@
     cost: typing.Optional[typing.Union[Cost, CostSpec]]
     price: typing.Optional[Amount]
     flag: typing.Optional[Flag]
     meta: typing.Optional[Meta]
 
 
 class Transaction(EntryBase):
-    entry_type: EntryType = Field(EntryType.TRANSACTION, const=EntryType.TRANSACTION)
+    entry_type: EntryType = Field(EntryType.TRANSACTION, const=True)
     flag: Flag
     payee: typing.Optional[str]
     narration: str
     tags: typing.Set[str]
     links: typing.Set[str]
     postings: typing.List[Posting]
 
 
 class Note(EntryBase):
-    entry_type: EntryType = Field(EntryType.NOTE, const=EntryType.NOTE)
+    entry_type: EntryType = Field(EntryType.NOTE, const=True)
     account: Account
     comment: str
     tags: typing.Set[str]
     links: typing.Set[str]
 
 
 class Event(EntryBase):
-    entry_type: EntryType = Field(EntryType.EVENT, const=EntryType.EVENT)
+    entry_type: EntryType = Field(EntryType.EVENT, const=True)
     type: str
     description: str
 
 
 class Price(EntryBase):
-    entry_type: EntryType = Field(EntryType.PRICE, const=EntryType.PRICE)
+    entry_type: EntryType = Field(EntryType.PRICE, const=True)
     currency: str
     amount: Amount
 
 
 class Document(EntryBase):
-    entry_type: EntryType = Field(EntryType.DOCUMENT, const=EntryType.DOCUMENT)
+    entry_type: EntryType = Field(EntryType.DOCUMENT, const=True)
     account: Account
     filename: str
     tags: typing.Set[str]
     links: typing.Set[str]
 
 
 class Custom(EntryBase):
-    entry_type: EntryType = Field(EntryType.CUSTOM, const=EntryType.CUSTOM)
+    entry_type: EntryType = Field(EntryType.CUSTOM, const=True)
     type: str
     values: typing.List[typing.Union[Amount, decimal.Decimal, str, bool]]
 
 
 EntryUnion = typing.Union[
     Open,
     Close,
```


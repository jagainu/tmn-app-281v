# tmn-shopping-list-240102

> **Status**: 🎨 DESIGNING

## 概要

ユーザーが買い物リストを簡単に作成、管理、共有できるWebアプリケーション。買い物アイテムの追加、編集、削除、チェックオフ機能を提供します。

## 機能

- [ ] アイテム追加
- [ ] アイテム編集
- [ ] アイテム削除
- [ ] アイテムチェックオフ
- [ ] リスト作成
- [ ] リスト共有

## 画面

| パス | 画面名 | 説明 |
|------|--------|------|
| `/` | ホーム | 買い物リストの一覧と新規リスト作成ボタン |
| `/list/[listId]` | リスト詳細 | 特定の買い物リストのアイテム表示と管理 |

## データ

### ShoppingList

| フィールド | 型 | 説明 |
|-----------|-----|------|
| id | string | リストの一意の識別子 |
| title | string | リストのタイトル |
| createdAt | string | リスト作成日時 |

### ShoppingListItem

| フィールド | 型 | 説明 |
|-----------|-----|------|
| id | string | アイテムの一意の識別子 |
| listId | string | 所属するリストのID |
| name | string | アイテム名 |
| quantity | number | 数量 |
| isChecked | boolean | アイテムがチェックされたかどうか |

## 認証

なし

---

## Tech Stack

- Framework: Next.js 14 (App Router)
- Styling: Tailwind CSS + shadcn/ui
- Database: Vercel KV
- Hosting: Vercel

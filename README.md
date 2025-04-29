# Proje Ekleme Formu (React + Supabase)

Bu proje, Supabase kullanarak proje verilerini veritabanına kaydeden basit bir React uygulamasıdır.

## Kurulum

```bash
npm install
npm start
```

## Yayınlamak İçin

```bash
npm run deploy
```

## Supabase Tablo Yapısı

```sql
create table projects (
  id uuid primary key default gen_random_uuid(),
  code text,
  name text,
  owner text,
  consultant text,
  start_date date,
  duration integer,
  end_date date,
  approved_extensions integer,
  contract_type text,
  contract_amount numeric,
  contract_currency text,
  total_approved_additions numeric,
  price_difference numeric,
  project_manager text,
  manager_contact text,
  address text,
  notes text,
  created_at timestamp with time zone default now()
);
```

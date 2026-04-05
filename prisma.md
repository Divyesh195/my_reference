# Prisma ORM

### 1. Schema Commands

#### Run this command after updating schema.prisma. It detects changes and generates SQL migration files (here neamed 'init'), applies it to your DB and auto runs 'prisma generate'

#### Important : use this in development mode, never use in production
```
npx prisma migrate dev --name init
```

#### Run this command anytime after changing scheme to enable type-safe queries in code. It regenerates prisma client. (safe for all environments)
```
npx prisma generate
```

#### Run this command to apply changes in DB directly without generating migration files (run 'npx prisma generate' afterwards)
```
npx prisma db push
```



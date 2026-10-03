# Credentials

Every declaration is signed by your Liccium installation. That signature shows which installation made the declaration, not who operates it. Verifiable Credentials close this gap: they are signed statements from a trusted issuer about you – for example that you control an email address or a domain, or that you are a member of an organisation.

When you add credentials, Liccium attaches them to every declaration automatically. Anyone looking up the declaration can then see who made the claim and which issuer vouches for it. For background, see Verifiable Creator Credentials and Trust Levels.

## Creator Credentials

Liccium Desktop works with [Creator Credentials](https://creatorcredentials.com/). To pair your installation:

1. Open Settings → Trust and choose Connect to Creator Credentials.
2. Sign in to Creator Credentials, or create an account.
3. Follow the three steps in Liccium to connect the account and import your credentials.

The credentials issued to you – for example Email, Domain, Member or Data Supplier credentials – are then included in your declarations.

## Declarations without credentials

Declarations without a credential are published as coming from an unverified declarer. They are still signed and timestamped, but others cannot connect them to a real-world identity.

## Removing a credential

You can remove a credential from Liccium at any time. It will no longer be attached to new declarations. Declarations you already published keep the credentials they were signed with.

## Self-verification – in development

A future release will let you sign in with Bluesky, LinkedIn, Apple ID or Google. Liccium will then issue a credential stating that the operator of your installation controls that account, signed under a certificate from an EU trust service.

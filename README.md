# Community Collaboration Message

## About Me

Hi there! I’m **Ch312 C3uZ**, also known as **H4ckD4D**, a cybersecurity expert, ethical hacker, and passionate protector of the most vulnerable among us: our children. Over the years, I’ve dedicated my skills to unmasking predators, dismantling networks of traffickers, and safeguarding families from exploitation. My work spans the realms of advanced AI-driven systems, cryptographic analysis, and hands-on operations that go beyond the digital world.

I believe that **technology, knowledge, and community collaboration** are our strongest weapons against those who prey on the innocent. My mission is clear: **to find and stop predators, rescue children, and create a safer world for them to thrive.**

## How You Can Join the Fight

I’m calling on hackers, developers, educators, and global citizens to collaborate in this crucial mission. Whether it’s through code, education, or advocacy, every contribution helps in the fight against child trafficking and predation.

### Ways to Contribute:
- **Code:** Help develop advanced tools to detect and prevent trafficking activities.
- **Educate:** Spread awareness about online safety and digital threats.
- **Advocate:** Share resources and support initiatives aimed at protecting children worldwide.

Together, we can make a difference.

---

### My Slogan
**"Predators and child traffickers, you will be found, and the children will be saved! This is my mission: to find you!"**


# FOFA Syntax Guide for OSINT Queries

This document outlines the syntax and usage examples for conducting FOFA queries. It includes basic, advanced, and unique filters tailored for cybersecurity and OSINT tasks.


## **Basic Queries**

| **Syntax** | **Example**                          | **Description**                | `=` | `!=` | `*=` |
|------------|--------------------------------------|--------------------------------|------|-------|------|
| `ip`       | `ip="1.1.1.1"`                      | Query by a single IPv4 address. | ✓   | ✓     | -    |
|            | `ip="220.181.111.1/24"`             | Query by IPv4 C segment.        | ✓   | ✓     | -    |
|            | `ip="2600:9000:202a:2600:18:4ab7:f600:93a1"` | Query by a single IPv6 address. | ✓   | ✓     | -    |
| `port`     | `port="6379"`                       | Query by open port number.      | ✓   | ✓     | ✓    |
| `domain`   | `domain="qq.com"`                   | Query by domain name.           | ✓   | ✓     | ✓    |
| `host`     | `host=".fofa.info"`                 | Query by hostname.              | ✓   | ✓     | ✓    |
| `os`       | `os="centos"`                       | Query by operating system.      | ✓   | ✓     | ✓    |
| `server`   | `server="Microsoft-IIS/10"`         | Query by server banner.         | ✓   | ✓     | ✓    |
| `asn`      | `asn="19551"`                       | Query by autonomous system number. | ✓   | ✓     | ✓    |
| `org`      | `org="LLC Baxet"`                   | Query by affiliated organization. | ✓   | ✓     | ✓    |

## **Special Labels**

| **Syntax**  | **Example**                          | **Description**                | `=` | `!=` | `*=` |
|-------------|--------------------------------------|--------------------------------|------|-------|------|
| `app`       | `app="Microsoft-Exchange"`           | Query by FOFA-organized fingerprints. | ✓ | -   | -    |
| `product`   | `product="NGINX"`                    | Query by product names tagged by FOFA. | ✓ | ✓   | -    |
| `category`  | `category="Service"`                 | Query by category (e.g., service). | ✓ | ✓   | -    |
| `type`      | `type="service"`                     | Filter protocol assets.         | ✓   | -     | -    |
| `is_cloud`  | `is_cloud=true`                      | Filter cloud service assets.    | ✓   | -     | -    |
| `is_honeypot` | `is_honeypot=true`                 | Filter honeypots (Professional tier). | ✓ | -   | -    |

## **Website-Specific Queries**

| **Syntax**      | **Example**                        | **Description**                | `=` | `!=` | `*=` |
|------------------|------------------------------------|--------------------------------|------|-------|------|
| `title`         | `title="beijing"`                  | Query by website title.        | ✓   | ✓     | ✓    |
| `header`        | `header="elastic"`                 | Query by HTTP response headers.| ✓   | ✓     | ✓    |
| `body`          | `body="google"`                    | Query by HTML body content.    | ✓   | ✓     | -    |
| `icon_hash`     | `icon_hash="-247388890"`           | Query by favicon hash.         | ✓   | ✓     | -    |
| `status_code`   | `status_code="402"`                | Filter services by HTTP status code. | ✓ | ✓   | -    |

## **Location Queries**

| **Syntax**   | **Example**             | **Description**                | `=` | `!=` | `*=` |
|--------------|-------------------------|--------------------------------|------|-------|------|
| `country`    | `country="US"`          | Query by country code.         | ✓   | ✓     | -    |
| `region`     | `region="New York"`     | Query by region or province.   | ✓   | ✓     | -    |
| `city`       | `city="Hangzhou"`       | Query by city name.            | ✓   | ✓     | -    |

## **Certificate Queries**

| **Syntax**          | **Example**                           | **Description**                | `=` | `!=` | `*=` |
|----------------------|---------------------------------------|--------------------------------|------|-------|------|
| `cert`              | `cert="baidu"`                       | Query by certificate content. | ✓   | ✓     | ✓    |
| `cert.subject`      | `cert.subject="Oracle Corporation"`  | Query by certificate subject. | ✓   | ✓     | ✓    |
| `cert.issuer`       | `cert.issuer="DigiCert"`             | Query by certificate issuer.  | ✓   | ✓     | ✓    |
| `cert.is_valid`     | `cert.is_valid=true`                 | Filter valid certificates.    | ✓   | -     | -    |
| `cert.is_expired`   | `cert.is_expired=true`               | Filter expired certificates.  | ✓   | -     | -    |

## **Time Filters**

| **Syntax** | **Example**              | **Description**                | `=` | `!=` | `*=` |
|------------|--------------------------|--------------------------------|------|-------|------|
| `after`    | `after="2023-01-01"`     | Filter by last updated after a date. | ✓ | -   | -    |
| `before`   | `before="2023-12-01"`    | Filter by last updated before a date. | ✓ | -   | -    |

---

Use this reference as a quick guide for efficient and precise FOFA queries. For more details, visit the official FOFA documentation.

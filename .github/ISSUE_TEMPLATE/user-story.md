---
name: User Story
about: Create a user story for the product catalog service
title: Catalog service user story
labels: enhancement
assignees: mitra9917
---

## As a
Product Manager

## I need
the ability to create, update, and retrieve products in the catalog

## So that
customers can view accurate and up-to-date product information and the business can manage products efficiently

---

## Details and Assumptions
- The catalog service exposes REST APIs
- Each product has an id, name, description, price, and availability status
- Only authenticated users can create or update products
- The system is expected to handle basic CRUD operations reliably

---

## Acceptance Criteria

```gherkin
Given an authenticated user
When the user submits valid product details
Then the product is successfully created in the catalog

Given an existing product in the catalog
When the user updates the product information
Then the updated product details are saved and retrievable

Given products exist in the catalog
When a user requests the product list
Then all available products are returned successfully

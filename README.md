# realm-io
How to use realm database using swift 💪🏻

## What is Realm
Realm is a cross-platform mobile object database. It’s very fast, performant and easy to use as compared to Core Data and Sqlite. It uses its storage mechanism to store object as JSON on disk as compared to Core Data that uses Sqlite as its backend. It is written in cross-platform C++ so it works exactly the same way on Android, iOS, macOS or any other platform.

## RealmSwift
Most of Realm is open-source, but the secret sauce behind Realm’s platform is the Core DB engine written from scratch in C++. RealmSwift is a wrapper around the Objective-C Realm framework and Objective-C Realm framework is a wrapper around Realm Core DB engine.

## Realm objects
Basically a standard data model, much like any other standard data model you’ve defined in your apps. The only difference is they’re backed by Realm persistence and abilities.
Every model you want to persist you have to inherit from Object class.

## Types
Since RealmSwift is a wrapper around the Objective-C Realm framework Types like (String, Date, Data)
are sub-classes of NSObject in Objective-C.
## @objc ⬇️:
means you want your Swift code (class, method, property, etc.) to be visible from Objective-C.
## dynamic ⬇️:
means you want to use Objective-C dynamic dispatch. To make simple swift object stores in database Realm uses Objective-C dynamic dispatch feature to do work under the hood.

dynamic is mandatory: ➡️ Yes, it is mandatory for normal var properties. From the realm docs.
Realm model properties need the dynamic var attribute in order for these properties to become accessors for the underlying database data.

## Relationships
test

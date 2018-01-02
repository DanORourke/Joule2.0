# Joule2.0

## Overview

Joule2.0 is a blockchain based cloud storage system.  The blockchain holds the hash of users data, and miners are rewarded for holding and serving the raw data to users.

The unit of currency is called a joule.  The txo that assigns a joule to a user also holds the hash of the stored information.

Joule2.0 uses a new type of consensus algorithm, called proof of work and service(POWAS).  A miner is granted the right to create the next block when he produces a mining hash less than the target hash.  A mining hash is a combination of a proof of work hash and a proof of service hash.  A proof of service hash is created by earning the signature of the owner of a joule and then appending the signature to the end of a unit of raw data referenced with a hash on a txo, and then hashing the result. This rewards the miner for keeping a users raw data and sending it to him upon request in exchange for an unlocking script that contains the signature of the previous header hash.
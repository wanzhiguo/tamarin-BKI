# tamarin proof for BKI protocol.
In this proof, strategies we adopt are:
   1. Secure channels are modelled between Domain and CAs with rules from tamarin manual.
   2. Log on blockchain is modelled as a list of records, and it is append-only;
   3. CAs' identities are modelled as '1', '1'+'1', '1'+'1'+'1', ...; There can be unlimited number of CAs.
   4. The model support any combination of k CAs to issue certs, any combination of t CAs to revoke certs.
   5. BLMs are modelled as single trusted BLM, as we assume the blockchain is securely maintained with consensus algorithms.

To run the proof:
   tamarin-prover --prove BKI-proof.spthy -Dsecure1 -Dsecure2

<!-- This markdown document is to lay out all of our elements and attributes in a visual way to allow optimized translation into schemas -->

### Entity Types
- state
- chamber
- committee
- executive
- person
- instrument

### Metadata Types
- constant <!-- things that generally don't change year to year -->
- point_in_time <!-- things that do or can change, sometimes derivable from constants -->

### Enumeration
- state
  - state_name <!-- constrained to set of states -->
  - state_meta_constant
    - state_cameral <!-- constrained to set of unicameral/bicameral -->
    - state_chambers <!-- conditional on state_cameral, constrained to unicameral/upper & lower -->
      - unicameral_chamber
        - number_of_members_statute
        - votes_to_pass_regular
        - votes_to_pass_emergency
        - votes_to_override_veto
        - standing_committees
      - upper_chamber
        - number_of_members_statute
        - votes_to_pass_regular
        - votes_to_pass_emergency
        - votes_to_override_veto
        - standing_committees
      - lower_chamber
        - number_of_members_statute
        - votes_to_pass_regular
        - votes_to_pass_emergency
        - votes_to_override_veto
        - standing_committees
    - state_executive
      - state_veto_type
    - state_sessions
      - 
    - state_uniques <!-- element for state quirks -->
    - state_meta_current   
    - state_chambers
        - unicameral_chamber
          - number_of_members_current
        - upper_chamber
          - number_of_members_current
        - lower_chamber
          - number_of_members_current
      
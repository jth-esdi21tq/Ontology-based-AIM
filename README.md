# Ontology-based-AIM-PM-BF
#Ontology-based AIM Case Study for Master Thesis in Product Development with a specialization in Sustainable Building Information Management

@prefix : <http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xml: <http://www.w3.org/XML/1998/namespace> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@base <http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11> .

<http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11> rdf:type owl:Ontology .

#################################################################
#    Annotation properties
#################################################################

###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#IsPointOf
:IsPointOf rdf:type owl:AnnotationProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#feeds
:feeds rdf:type owl:AnnotationProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#hasAddress
:hasAddress rdf:type owl:AnnotationProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#hasLocation
:hasLocation rdf:type owl:AnnotationProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#hasPart
:hasPart rdf:type owl:AnnotationProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#hasPoint
:hasPoint rdf:type owl:AnnotationProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#hasTag
:hasTag rdf:type owl:AnnotationProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#hasUnit
:hasUnit rdf:type owl:AnnotationProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#isFedBy
:isFedBy rdf:type owl:AnnotationProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#isLocationOf
:isLocationOf rdf:type owl:AnnotationProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#isPartOf
:isPartOf rdf:type owl:AnnotationProperty .


#################################################################
#    Object Properties
#################################################################

###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#operationalStageCount
:operationalStageCount rdf:type owl:ObjectProperty .


#################################################################
#    Data properties
#################################################################

###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#grad_celsius
:grad_celsius rdf:type owl:DatatypeProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#lux
:lux rdf:type owl:DatatypeProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#people
:people rdf:type owl:DatatypeProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#percentage
:percentage rdf:type owl:DatatypeProperty .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#ppm
:ppm rdf:type owl:DatatypeProperty .


#################################################################
#    Classes
#################################################################

###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Air_Handling_Unit
:Air_Handling_Unit rdf:type owl:Class ;
                   rdfs:subClassOf :HVAC_Equipment ;
                   rdfs:comment "Assembly consisting of sections containing a fan or fans and other necessary equipment to perform one or more of the following functions: circulating, filtration, heating, cooling, heat recovery, humidifying, dehumidifying, and mixing of air. Is usually connected to an air-distribution system."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Air_Quality_Sensor
:Air_Quality_Sensor rdf:type owl:Class ;
                    rdfs:subClassOf :Sensor ;
                    rdfs:comment "A sensor which provides a measure of air quality"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Air_Temperature_Alarm
:Air_Temperature_Alarm rdf:type owl:Class ;
                       rdfs:subClassOf :Temperature_Alarm ;
                       rdfs:comment "An alarm that indicates the off-normal conditions associated with the temperature of air."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Air_Temperature_Setpoint
:Air_Temperature_Setpoint rdf:type owl:Class ;
                          rdfs:subClassOf :Temperature_Setpoint ;
                          rdfs:comment "Sets temperature of air"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Alarm
:Alarm rdf:type owl:Class ;
       rdfs:subClassOf :Point ;
       rdfs:comment "Alarm points are signals (either audible or visual) that alert an operator to an off-normal condition which requires some form of corrective action"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Automated_External_Defibrillator
:Automated_External_Defibrillator rdf:type owl:Class ;
                                  rdfs:subClassOf :Safety_Equipment .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Blind
:Blind rdf:type owl:Class ;
       rdfs:subClassOf :Shading_Equipment ;
       rdfs:comment "A window covering."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Breaker_Panel
:Breaker_Panel rdf:type owl:Class ;
               rdfs:subClassOf :Electrical_Equipment ;
               rdfs:comment "Breaker Panel distributes power into various end-uses."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Building
:Building rdf:type owl:Class ;
          rdfs:subClassOf :Location ;
          rdfs:comment "An independent unit of the built environment with a characteristic spatial structure, intended to serve at least one function or user activity [ISO 12006-2:2013]"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#CO2_Alarm
:CO2_Alarm rdf:type owl:Class ;
           rdfs:subClassOf :Alarm ;
           rdfs:comment "An alarm that indicates the off-normal conditions associated with the presence of carbon dioxide."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#CO2_Sensor
:CO2_Sensor rdf:type owl:Class ;
            rdfs:subClassOf :Air_Quality_Sensor ;
            rdfs:comment "Measures properties of CO2 in air"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#CO2_Setpoint
:CO2_Setpoint rdf:type owl:Class ;
              rdfs:subClassOf :Setpoint ;
              rdfs:comment "Sets some property of CO2"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Conference_Room
:Conference_Room rdf:type owl:Class ;
                 rdfs:subClassOf :Room ;
                 rdfs:comment "A space dedicated in which to hold meetings"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Damper
:Damper rdf:type owl:Class ;
        rdfs:subClassOf :HVAC_Equipment ;
        rdfs:comment "Element inserted into an air-distribution system or element of an air-distribution system permitting modification of the air resistance of the system and consequently changing the airflow rate or shutting off the airflow."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Disconnect_Switch
:Disconnect_Switch rdf:type owl:Class ;
                   rdfs:subClassOf :Electrical_Equipment ;
                   rdfs:comment "Building power is most commonly provided by utility company through a master disconnect switch (sometimes called a service disconnect) in the main electrical room of a building. The Utility Company provided master disconnect switch often owns or restricts access to this switch. There can also be other cases where a disconnect is placed into an electrical system to allow service cut-off to a portion of the building."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Electrical_Equipment
:Electrical_Equipment rdf:type owl:Class ;
                      rdfs:subClassOf :Equipment .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Equipment
:Equipment rdf:type owl:Class ;
           rdfs:comment "Devices that serve all or part of the building and may include electric power, lighting, transportation, or service water heating, including, but not limited to, furnaces, boilers, air conditioners, heat pumps, chillers, water heaters, lamps, luminaires, ballasts, elevators, escalators, or other devices or installations."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Fire_Alarm
:Fire_Alarm rdf:type owl:Class ;
            rdfs:subClassOf :Fire_Safety_Equipment .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Fire_Safety_Equipment
:Fire_Safety_Equipment rdf:type owl:Class ;
                       rdfs:subClassOf :Equipment .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#First_Aid_Kit
:First_Aid_Kit rdf:type owl:Class ;
               rdfs:subClassOf :Safety_Equipment .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Floor
:Floor rdf:type owl:Class ;
       rdfs:subClassOf :Location ;
       rdfs:comment "A level, typically representing a horizontal aggregation of spaces that are vertically bound. (referring to IFC)"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Furniture
:Furniture rdf:type owl:Class ;
           rdfs:subClassOf :Equipment ;
           rdfs:comment "Movable objects intended to support various human activities such as seating, eating and sleeping" .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#HVAC_Equipment
:HVAC_Equipment rdf:type owl:Class ;
                rdfs:subClassOf :Equipment ;
                rdfs:comment "The equipment, distribution systems and terminals that provide, either collectively or individually, the processes of heating, ventilating or air conditioning to a building or portion of a building"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#HVAC_Zone
:HVAC_Zone rdf:type owl:Class ;
           rdfs:subClassOf :Zone ;
           rdfs:comment "A space or group of spaces, within a building with heating, cooling, and ventilating requirements, that are sufficiently similar so that desired conditions (e.g., temperature) can be maintained throughout using a single sensor (e.g., thermostat or temperature sensor)."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Heat_Detector
:Heat_Detector rdf:type owl:Class ;
               rdfs:subClassOf :Fire_Safety_Equipment .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Humidity_Alarm
:Humidity_Alarm rdf:type owl:Class ;
                rdfs:subClassOf :Alarm ;
                rdfs:comment "An alarm that indicates the off-normal conditions associated with the concentration of water vapor in the air."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Humidity_Sensor
:Humidity_Sensor rdf:type owl:Class ;
                 rdfs:subClassOf :Sensor ;
                 rdfs:comment "Measures the concentration of water vapor in air"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Humidity_Setpoint
:Humidity_Setpoint rdf:type owl:Class ;
                   rdfs:subClassOf :Setpoint ;
                   rdfs:comment "Sets humidity"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Illuminance_Sensor
:Illuminance_Sensor rdf:type owl:Class ;
                    rdfs:subClassOf :Sensor ;
                    rdfs:comment "Measures the total luminous flux incident on a surface, per unit area"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Inverter
:Inverter rdf:type owl:Class ;
          rdfs:subClassOf :Electrical_Equipment ;
          rdfs:comment "A device that changes direct current into alternating current"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Lighting_Zone
:Lighting_Zone rdf:type owl:Class ;
               rdfs:subClassOf :Zone .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Lightning
:Lightning rdf:type owl:Class ;
           rdfs:subClassOf :Lightning_Equipment .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Lightning_Equipment
:Lightning_Equipment rdf:type owl:Class ;
                     rdfs:subClassOf :Equipment .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Location
:Location rdf:type owl:Class .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Luminaire
:Luminaire rdf:type owl:Class ;
           rdfs:subClassOf :Lightning ;
           rdfs:comment "A complete lighting unit consisting of a lamp or lamps and ballast(s) (when applicable) together with the parts designed to distribute the light, to position and protect the lamps, and to connect the lamps to the power supply."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Luminaire_Driver
:Luminaire_Driver rdf:type owl:Class ;
                  rdfs:subClassOf :Lightning ;
                  rdfs:comment "A power source for a luminaire"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Motion_Sensor
:Motion_Sensor rdf:type owl:Class ;
               rdfs:subClassOf :Sensor ;
               rdfs:comment "Detects the presence of motion in some area"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Occupancy_Sensor
:Occupancy_Sensor rdf:type owl:Class ;
                  rdfs:subClassOf :Sensor ;
                  rdfs:comment "Detects occupancy of some space or area"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Occupancy_Status
:Occupancy_Status rdf:type owl:Class ;
                  rdfs:subClassOf :Status ;
                  rdfs:comment "Indicates if a room or space is occupied"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#PlugStrip
:PlugStrip rdf:type owl:Class ;
           rdfs:subClassOf :Electrical_Equipment ;
           rdfs:comment "A device containing a block of electrical sockets allowing multiple electrical devices to be powered from a single electrical socket."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Point
:Point rdf:type owl:Class .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Room
:Room rdf:type owl:Class ;
      rdfs:subClassOf :Space ;
      rdfs:comment "Base class for all more specific room types."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Safety_Equipment
:Safety_Equipment rdf:type owl:Class ;
                  rdfs:subClassOf :Equipment .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Sensor
:Sensor rdf:type owl:Class ;
        rdfs:subClassOf :Point ;
        rdfs:comment "A Sensor is an input point that represents the value of a device or instrument designed to detect and measure a variable (ASHRAE Dictionary)."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Setpoint
:Setpoint rdf:type owl:Class ;
          rdfs:subClassOf :Point ;
          rdfs:comment "A Setpoint is an input value at which the desired property is set"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Shading_Equipment
:Shading_Equipment rdf:type owl:Class ;
                   rdfs:subClassOf :Equipment .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Smoke_Detector
:Smoke_Detector rdf:type owl:Class ;
                rdfs:subClassOf :Fire_Safety_Equipment .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Space
:Space rdf:type owl:Class ;
       rdfs:subClassOf :Location ;
       rdfs:comment "A part of the physical world or a virtual world whose 3D spatial extent is bounded actually or theoretically, and provides for certain functions within the zone it is contained in."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Space_Heater
:Space_Heater rdf:type owl:Class ;
              rdfs:subClassOf :HVAC_Equipment ;
              rdfs:comment "A heater used to warm the air in an enclosed area, such as a room or office"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Status
:Status rdf:type owl:Class ;
        rdfs:subClassOf :Point ;
        rdfs:comment "A Status is input point that reports the current operating mode, state, position, or condition of an item. Statuses are observations and should be considered 'read-only'"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Temperature_Alarm
:Temperature_Alarm rdf:type owl:Class ;
                   rdfs:subClassOf :Alarm ;
                   rdfs:comment "An alarm that indicates the off-normal conditions associated with temperature."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Temperature_Sensor
:Temperature_Sensor rdf:type owl:Class ;
                    rdfs:subClassOf :Sensor ;
                    rdfs:comment "Measures temperature: the physical property of matter that quantitatively expresses the common notions of hot and cold"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Temperature_Setpoint
:Temperature_Setpoint rdf:type owl:Class ;
                      rdfs:subClassOf :Setpoint ;
                      rdfs:comment "Sets temperature"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Thermostat
:Thermostat rdf:type owl:Class ;
            rdfs:subClassOf :HVAC_Equipment ;
            rdfs:comment "An automatic control device used to maintain temperature at a fixed or adjustable setpoint."^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#Zone
:Zone rdf:type owl:Class ;
      rdfs:subClassOf :Location ;
      rdfs:comment "(1) a separately controlled heated or cooled space. (2) one occupied space or several occupied spaces with similar occupancy category, occupant density, zone air distribution effectiveness, and zone primary airflow per unit area. (3) space or group of spaces within a building for which the heating, cooling, or lighting requirements are sufficiently similar that desired conditions can be maintained throughout by a single controlling device."^^xsd:string .


#################################################################
#    Individuals
#################################################################

###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ00_air_handling_unit
:EQ00_air_handling_unit rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ00_automated_external_defibrilator
:EQ00_automated_external_defibrilator rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ00_blind
:EQ00_blind rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ00_breaker_panel
:EQ00_breaker_panel rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ00_damper
:EQ00_damper rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ00_disconnect_switch
:EQ00_disconnect_switch rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ00_first_aid_kit
:EQ00_first_aid_kit rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ00_heat_detector
:EQ00_heat_detector rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ00_inverter
:EQ00_inverter rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ00_plugstrip
:EQ00_plugstrip rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ00_space_heater
:EQ00_space_heater rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ00_thermostat
:EQ00_thermostat rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ01_conference_chair_collection
:EQ01_conference_chair_collection rdf:type owl:NamedIndividual ,
                                           :Furniture ;
                                  :operationalStageCount :EQ01_conference_chair_collection ;
                                  :hasLocation :LOC01_conference_room ;
                                  :hasTag "EQ01 conference chair collection"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ01_conference_table
:EQ01_conference_table rdf:type owl:NamedIndividual ,
                                :Furniture ;
                       :operationalStageCount :EQ01_conference_table ;
                       :hasLocation :LOC01_conference_room ;
                       :hasTag "EQ01 conference table"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ01_fire_alarm
:EQ01_fire_alarm rdf:type owl:NamedIndividual ,
                          :Fire_Alarm ;
                 :feeds :EQ01_fire_safety_equipment ;
                 :hasLocation :LOC01_conference_room ;
                 :hasTag "EQ01 fire alarm"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ01_fire_safety_equipment
:EQ01_fire_safety_equipment rdf:type owl:NamedIndividual ,
                                     :Fire_Safety_Equipment ;
                            :IsPointOf :LOC01_conference_room_zone ;
                            :isFedBy :EQ01_fire_alarm ,
                                     :EQ01_smoke_detector .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ01_luminaire_collection
:EQ01_luminaire_collection rdf:type owl:NamedIndividual ,
                                    :Luminaire ;
                           :feeds :LOC01_lightning_zone ;
                           :hasLocation :LOC01_conference_room ;
                           :hasPart :EQ01_luminaire_driver ;
                           :hasTag "EQ01 luminaire collection"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ01_luminaire_driver
:EQ01_luminaire_driver rdf:type owl:NamedIndividual ,
                                :Luminaire_Driver ;
                       :isPartOf :EQ01_luminaire_collection .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#EQ01_smoke_detector
:EQ01_smoke_detector rdf:type owl:NamedIndividual ,
                              :Smoke_Detector ;
                     :feeds :EQ01_fire_safety_equipment ;
                     :hasLocation :LOC01_conference_room ;
                     :hasTag "EQ01 smoke detector"^^xsd:string .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#LOC00_HVAC_zone
:LOC00_HVAC_zone rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#LOC01_building_use_case
:LOC01_building_use_case rdf:type owl:NamedIndividual ,
                                  :Building ;
                         :hasAddress "Building Sample Address"^^xsd:string ;
                         :hasPart :LOC_floor_1 ,
                                  :LOC_floor_2 ,
                                  :LOC_floor_3 ,
                                  :LOC_floor_4 ,
                                  :LOC_floor_5 .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#LOC01_conference_room
:LOC01_conference_room rdf:type owl:NamedIndividual ,
                                :Conference_Room ;
                       :hasLocation :LOC01_conference_room_zone ,
                                    :LOC01_lightning_zone ;
                       :hasTag "LOC01 conference room"^^xsd:string ;
                       :isLocationOf :EQ01_conference_chair_collection ,
                                     :EQ01_conference_table ,
                                     :EQ01_fire_alarm ,
                                     :EQ01_luminaire_collection ,
                                     :EQ01_smoke_detector ,
                                     :POINT01_air_quality_sensor ,
                                     :POINT01_co2_sensor ,
                                     :POINT01_humidity_sensor ,
                                     :POINT01_illuminance_sensor ,
                                     :POINT01_motion_sensor ,
                                     :POINT01_occupancy_sensor ,
                                     :POINT01_temperature_sensor ;
                       :isPartOf :LOC01_conference_room_zone ,
                                 :LOC01_lightning_zone .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#LOC01_conference_room_zone
:LOC01_conference_room_zone rdf:type owl:NamedIndividual ,
                                     :Zone ;
                            :hasPart :LOC01_conference_room ;
                            :hasPoint :EQ01_fire_safety_equipment ,
                                      :POINT01_air_quality_sensor ,
                                      :POINT01_co2_sensor ,
                                      :POINT01_humidity_sensor ,
                                      :POINT01_illuminance_sensor ,
                                      :POINT01_motion_sensor ,
                                      :POINT01_occupancy_sensor ,
                                      :POINT01_temperature_sensor ;
                            :isPartOf :LOC_floor_1 .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#LOC01_lightning_zone
:LOC01_lightning_zone rdf:type owl:NamedIndividual ,
                               :Lighting_Zone ;
                      :hasPart :LOC01_conference_room ;
                      :isFedBy :EQ01_luminaire_collection ;
                      :isPartOf :LOC_floor_1 .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#LOC_floor_1
:LOC_floor_1 rdf:type owl:NamedIndividual ,
                      :Floor ;
             :hasPart :LOC01_conference_room_zone ,
                      :LOC01_lightning_zone ;
             :isPartOf :LOC01_building_use_case .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#LOC_floor_2
:LOC_floor_2 rdf:type owl:NamedIndividual ;
             :isPartOf :LOC01_building_use_case .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#LOC_floor_3
:LOC_floor_3 rdf:type owl:NamedIndividual ;
             :isPartOf :LOC01_building_use_case .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#LOC_floor_4
:LOC_floor_4 rdf:type owl:NamedIndividual ;
             :isPartOf :LOC01_building_use_case .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#LOC_floor_5
:LOC_floor_5 rdf:type owl:NamedIndividual ;
             :isPartOf :LOC01_building_use_case .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT00_air_temperature_alarm
:POINT00_air_temperature_alarm rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT00_air_temperature_setpoint
:POINT00_air_temperature_setpoint rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT00_co2_alarm
:POINT00_co2_alarm rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT00_co2_setpoint
:POINT00_co2_setpoint rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT00_humidity_alarm
:POINT00_humidity_alarm rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT00_humidity_setpoint
:POINT00_humidity_setpoint rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT00_occupancy_status
:POINT00_occupancy_status rdf:type owl:NamedIndividual .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT01_air_quality_sensor
:POINT01_air_quality_sensor rdf:type owl:NamedIndividual ,
                                     :Air_Quality_Sensor ;
                            :ppm ""^^xsd:double ;
                            :IsPointOf :LOC01_conference_room_zone ;
                            :hasLocation :LOC01_conference_room ;
                            :hasTag "POINT01 air quality sensor"^^xsd:string ;
                            :hasUnit :ppm .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT01_co2_sensor
:POINT01_co2_sensor rdf:type owl:NamedIndividual ,
                             :CO2_Sensor ;
                    :ppm ""^^xsd:double ;
                    :IsPointOf :LOC01_conference_room_zone ;
                    :hasLocation :LOC01_conference_room ;
                    :hasTag "POINT01 co2 sensor"^^xsd:string ;
                    :hasUnit :ppm .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT01_humidity_sensor
:POINT01_humidity_sensor rdf:type owl:NamedIndividual ,
                                  :Humidity_Sensor ;
                         :percentage ""^^xsd:int ;
                         :IsPointOf :LOC01_conference_room_zone ;
                         :hasLocation :LOC01_conference_room ;
                         :hasTag "POINT01 humidity sensor"^^xsd:string ;
                         :hasUnit :percentage .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT01_illuminance_sensor
:POINT01_illuminance_sensor rdf:type owl:NamedIndividual ,
                                     :Illuminance_Sensor ;
                            :lux ""^^xsd:double ;
                            :IsPointOf :LOC01_conference_room_zone ;
                            :hasLocation :LOC01_conference_room ;
                            :hasTag "POINT01 illuminance sensor"^^xsd:string ;
                            :hasUnit :lux .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT01_motion_sensor
:POINT01_motion_sensor rdf:type owl:NamedIndividual ,
                                :Motion_Sensor ;
                       owl:topDataProperty "false"^^xsd:boolean ;
                       :IsPointOf :LOC01_conference_room_zone ;
                       :hasLocation :LOC01_conference_room ;
                       :hasTag "POINT01 motion sensor"^^xsd:string ;
                       :hasUnit "false"^^xsd:boolean .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT01_occupancy_sensor
:POINT01_occupancy_sensor rdf:type owl:NamedIndividual ,
                                   :Occupancy_Sensor ;
                          :people ""^^xsd:int ;
                          :IsPointOf :LOC01_conference_room_zone ;
                          :hasLocation :LOC01_conference_room ;
                          :hasTag "POINT01 occupancy sensor"^^xsd:string ;
                          :hasUnit :people .


###  http://www.semanticweb.org/desgi/ontologies/2023/2/untitled-ontology-11#POINT01_temperature_sensor
:POINT01_temperature_sensor rdf:type owl:NamedIndividual ,
                                     :Temperature_Sensor ;
                            :grad_celsius ""^^xsd:double ;
                            :IsPointOf :LOC01_conference_room_zone ;
                            :hasLocation :LOC01_conference_room ;
                            :hasTag "POINT01 temperature sensor"^^xsd:string ;
                            :hasUnit :grad_celsius .


[ rdfs:comment :operationalStageCount
] .

###  Generated by the OWL API (version 4.5.9.2019-02-01T07:24:44Z) https://github.com/owlcs/owlapi

				DECLARE
						l_selected APEX_APPLICATION_GLOBAL.VC_ARR2;
                        N_selected APEX_APPLICATION_GLOBAL.VC_ARR2;
							BEGIN
						l_selected := APEX_UTIL.STRING_TO_TABLE(:P1_ITEM);
                        N_selected := APEX_UTIL.STRING_TO_TABLE(:P2_ITEM);
						FOR i in 1..l_selected.count
							LOOP
                            FOR r in reverse 1..N_selected.count
							LOOP
						INSERT INTO TABLE(P1_COLUMN, P3_COLUMN, P2_COLUMN)
						VALUES (l_selected(i), :P3_ITEM, N_selected(r));
						END LOOP;
                        END LOOP;
						END;




